---
title: 如何使用 Spring Boot，Neon Postgres 和 Azure App 服务开发 CRUD 应用
date: 2024-07-28T07:47:06.061Z
author: Abhinav Pandey
authorURL: https://www.freecodecamp.org/news/author/abhinav-pandey/
OriginalURL: https://www.freecodecamp.org/news/build-a-crud-app-spring-boot-neon-postgres/
Proofreader: ""

---

在本文中，我们将探讨如何使用 Spring Boot 和 [Neon Postgres][1] 开发一个 CRUD（创建、读取、更新、删除）应用程序。

<!-- more -->

我们还将部署该应用程序到 [Azure App 服务][2]，并通过设置自动扩展和多环境等功能使其达到生产准备状态。

您还将了解 Neon Postgres 如何简化您的开发和部署过程。

## 我们将涵盖以下内容：

-   设置 Neon Postgres 数据库并探索其功能
-   使用 Spring Boot 构建一个 CRUD 应用并将其部署到 Azure App 服务
-   为什么 Neon 适合自动扩展的基础设施
-   Neon Postgres 中的数据库分支及其如何简化开发工作流程

## 前提条件

-   熟悉 Java、Maven 和 Spring Boot
-   基本的 SQL 数据库知识
-   理解无服务器和云服务
-   熟悉测试和部署过程

## 目录

-   [什么是 Neon Postgres？][3]
-   [如何设置数据库][4]
    -   [创建数据库][5]
-   [如何构建 Spring Boot CRUD 应用][6]
    -   [创建实体类][7]
    -   [创建仓库][8]
    -   [创建 REST 控制器][9]
    -   [配置数据库][10]
-   [如何部署到 Azure App 服务][11]
    -   [创建一个新的 Web 应用][12]
    -   [部署应用程序][13]
    -   [访问应用程序][14]
-   [如何设置自动扩展][15]
    -   [Azure 中的自动扩展][16]
    -   [Neon 中的自动扩展][17]
-   [如何在 Neon 配置数据库分支][18]
-   [总结][19]

## 什么是 Neon Postgres？

Neon 是一个完全托管的无服务器 Postgres 数据库平台。它提供高可用性、自动备份和扩展选项，以处理不同的流量水平。

Neon 旨在实现成本效益并对开发者友好，并专注于为开发者提供无缝体验。

除了标准的 Postgres 功能外，它还提供诸如数据库分支功能，使您能够为不同目的创建类似 Git 分支的数据库。

## 如何设置数据库

首先，让我们探索如何为您的应用程序设置一个 Neon 数据库。

首先，您需要在 Neon 网站上 [创建一个账户][20]。无需信用卡即可注册，并且系统会自动为您设置免费层以便开始。

这里有一个 Neon 计划的 [价格和功能比较][21]：

![Neon 计划的价格和功能比较截图](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Finxumg46sf92ffre6l2q.png)

Neon 价格计划

在免费层中，我们获得了 0.5 GB 的存储和基本计算资源，这足以玩转数据库并构建小型应用程序。

### 创建数据库

注册后，您可以访问仪表板并创建新项目。

首先填写项目名称、区域和 Postgres 版本选项。除此之外，我们还可以选择两个额外的选项：

-   **计算大小** – 您可以为数据库选择最小和最大计算大小。这对于根据负载自动扩展数据库很有用。
-   **中止时间** – 您可以设置一个时间，如果数据库未被使用将在该时间后暂停。这对于在数据库未被使用时节省成本很有用。

![创建数据库时所需填写的表单](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fggwuvqtb8ydl3mxd1dak.png)

在 Neon 中创建数据库项目

提交表单后，Neon 将创建数据库并提供连接详细信息。

![Neon 仪表板显示项目已准备就绪，并显示连接详细信息。](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fwe2x5d81euphg2owgxhd.png)

Neon 仪表板

如您所见，数据库在 3.3 秒内设立完毕（相比需要数小时来安装和设置自己的基础设施）。您可以选择多种方式连接到数据库。在本教程中，选择 Java 作为编程语言并获取 JDBC 连接字符串。

## 如何构建 Spring Boot CRUD 应用

接下来，让我们设置我们的 CRUD 应用。我们将使用 Spring Boot，因为它提供了构建 web 应用程序的简单启动和配置。

我们可以使用 [Spring Initializr][22] 生成一个带有必要依赖的新 Spring Boot 项目：

-   Spring Web – 用于构建 web 应用程序
-   Spring Data JPA – 用于使用 JPA 处理数据库
-   PostGres 驱动程序 – 用于连接到 Postgres 数据库

创建一个使用 Spring Initializer 的 Spring Boot 项目

你可以生成、下载项目并将其导入到你喜欢的 IDE 中。

### 创建一个实体类

让我们创建一个实体类来表示应用程序中的数据。首先，创建一个 `User` 类：

```Java
@Entity(name = "users")
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String name;
    private String email;

    // Constructors, Getters and Setters
}
```

实体名称 `users` 是你希望在数据库中使用的表的名称。

### 创建 Repository

接下来，创建一个与数据库交互的 repository 接口。你需要扩展 Spring Data JPA 提供的 `JpaRepository` 接口：

```Java
@Repository
public interface UserRepository extends JpaRepository<User, Long> {
}
```

你需要使用 `@Repository` 注解来标记这个接口为一个 Spring bean。`JpaRepository` 接口提供 `save`、`findAll`、`findById`、`delete` 等 CRUD 操作的方法，因此你不需要手动编写查询。

你将提供你的实体类 `User` 和主键类型 `Long` 作为 `JpaRepository` 接口的类型参数。

### 创建一个 REST 控制器

最后，创建一个 REST 控制器来处理 CRUD 操作。你将把 `UserRepository` 注入到控制器中并实现必要的端点：

```Java
@RestController
@RequestMapping("/users")
public class UserController {
    private final UserRepository userRepository;

    public UserController(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    @GetMapping
    public List<User> getUsers() {
        return userRepository.findAll();
    }

    @PostMapping
    public User createUser(@RequestBody User user) {
        return userRepository.save(user);
    }

    @PutMapping("/{id}")
    public User updateUser(@PathVariable Long id, @RequestBody User user) {
        user.setId(id);
        return userRepository.save(user);
    }

    @DeleteMapping("/{id}")
    public void deleteUser(@PathVariable Long id) {
        userRepository.deleteById(id);
    }
}
```

这里有一些注意事项：

-   使用 `@RestController` 注解来标记这个类为一个处理 REST 请求的控制器。
-   `@RequestMapping` 注解指定端点的基础 URL。
-   使用构造函数注入将 `UserRepository` 注入到控制器中。
-   最后，使用 `@GetMapping`、`@PostMapping`、`@PutMapping` 和 `@DeleteMapping` 注解实现 CRUD 操作的 API 端点。

### 配置数据库

要将你的 Spring Boot 应用程序连接到 Neon Postgres 数据库，你需要在 `application.properties` 文件中配置数据库 URL、用户名和密码：

```
spring.datasource.url=jdbc:postgresql://<db-url>/<db-name>?sslmode=require
spring.datasource.username=<username>
spring.datasource.password=<password>
spring.jpa.hibernate.ddl-auto=update
```

这里，你配置了 Neon 在创建数据库时提供的数据库 URL、用户名和密码。`spring.jpa.hibernate.ddl-auto=update` 属性告诉 Spring Boot 在应用程序启动时根据实体类自动创建必要的表或列。

## 如何在 Azure 应用服务上部署

现在你的 Spring Boot 应用程序已经准备好，是时候在 Azure 应用服务上部署它了。

### 创建一个新的 Web 应用

要将你的 Spring Boot 应用程序部署到 Azure 应用服务，你首先需要创建一个新的 `Web 应用`。你可以通过 Azure 门户按照以下步骤创建：

-   登录到 [Azure 门户][23]。
-   点击 `创建资源` 按钮。
-   搜索 `Web 应用` 并选择 `创建` 选项。
-   填写资源组、应用名称、运行时堆栈和区域等必要的详细信息。
-   点击 `查看 + 创建` 按钮。

![在 Azure 中创建 Web 应用的表单](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Flf2kmh12t8eucd1qa1pg.png)

在 Azure 中创建 Web 应用

### 部署应用程序

Web 应用大约需要几分钟的时间来创建。完成后，你可以将你的 Spring Boot 应用程序部署到 Azure 应用服务。

其中一种最简单的部署方法是将你的 Spring Boot 应用程序打包为 JAR 文件，并使用 Azure CLI 将其部署到 Azure 应用服务。

为此，请运行以下命令：

```
mvn package
az webapp deploy --src-path neon-demo-0.0.1-SNAPSHOT.jar --resource-group learn-ba1a439c-71ca-4cab-9bb1-f5b1331bab04 --name neon-app
```

这里，你使用 Maven 打包你的 Spring Boot 应用程序，并使用 Azure CLI 将 JAR 文件部署到 Azure 应用服务。你提供了 JAR 文件的路径、资源组和之前配置的应用名称。

### 访问应用程序

部署完成后，你可以通过导航到 Web 应用的 URL 访问你的 Spring Boot 应用程序。你的应用可在 `neon-app.azurewebsites.net` 访问。

#### 创建用户

```
curl -X POST -d '{"name":"John Doe","email":"john@gmail.com"}' https://neon-app.azurewebsites.net/users
```

在这里，您提供以 JSON 格式编写的用户数据来创建一个新用户。

#### 获取用户

您还可以通过获取所有用户来验证用户是否已创建：

```
curl -X GET https://neon-app.azurewebsites.net/users
```

## 如何设置自动扩展

在生产环境中，应用程序可能会遇到不同程度的流量，因此根据负载动态扩展应用程序非常重要。

让我们开始探索如何在需要时自动扩展您的应用程序。

### 在 Azure 中的自动扩展

Azure 应用服务提供了[自动扩展选项][24]，允许您根据需要自动调整实例数量。

您可以通过以下步骤在 Azure 门户中配置自动扩展规则：

-   在 Azure 门户中导航到 Web 应用。
-   从左侧菜单中单击`横向扩展（应用服务计划）`选项。
-   配置自动扩展规则——可以选择预定义的规则（如流量）或基于 CPU 使用率、内存使用率或自定义度量指标创建自定义规则。
-   保存。

Azure 会根据配置的规则自动扩展应用程序。

### 在 Neon 中的自动扩展

由于您的应用程序可根据负载自动扩展，因此您需要确保数据库能够处理增加的流量。

Neon 提供了[自动扩展选项][25]，以根据负载动态扩展数据库。您可以在 Neon 仪表板中配置自动扩展规则，以确保数据库能够处理增加的负载。

按以下步骤配置 Neon 的自动扩展：

1.  导航到 Neon 仪表板并选择数据库。然后选择分支以配置自动扩展。

![Neon 项目仪表板，重点展示分支部分](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fl6s84pqhk2avflpjbgrf.png)

在 Neon 项目仪表板中选择一个分支

2\.  单击 `Compute` 部分旁边的 `Edit` 按钮。基于 CPU 使用率、内存使用率或自定义度量指标配置自动扩展规则。

![Neon 中分支详细信息视图，重点展示 compute 部分的编辑按钮](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Ffkn11nop1zz9xxbfamsr.png)

Neon 中的分支详细信息视图

3\.  配置最小-最大计算大小并保存。当需要时，Neon 会根据配置的规则自动扩展数据库。

![启用自动扩展并选择计算的最小和最大大小的表单](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fdmuow8zvndz0dibv2kxt.png)

为计算设置自动扩展

确保应用程序和数据库可以根据负载动态扩展有助于高效处理不同级别的流量。

## 如何在 Neon 中配置数据库分支

在典型的开发工作流中，可能会使用多个数据库用于不同的目的，例如开发、测试和生产。

Neon Postgres 提供了[数据库分支][26]功能，可以为不同的用途创建多个分支。每个分支是独立使用的数据库实例。

这个类似 Git 的功能有助于为不同的环境（如开发、预生产和生产）设置数据库副本。它还有助于保存不同版本应用程序的数据。

让我们探索如何在 Neon Postgres 中创建和管理分支：

-   导航到 Neon 仪表板并选择数据库。
-   在 `Branches` 部分，点击 `View All` 按钮。
-   可以通过点击 `Create Branch` 按钮从现有分支创建一个新分支。您需要提供分支名称和要从父分支复制的数据。

![显示创建分支选项的分支视图](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F9ncdgdrj32etd3gbqurf.png)

创建分支选项

-   您可以选择复制所有数据，复制到某个时间点或特定记录。这对于多种用途，如恢复数据、创建新环境或测试新功能非常有用。

![从现有分支创建新分支](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fw7gchucru5qw294icqw3.png)

从现有分支创建新分支

-   Neon 会创建一个可以独立使用的新数据库分支。您可以在仪表板上找到新分支的 URL、用户名和密码。而且这一过程是在不产生任何停机时间和延迟的情况下实时完成的。

![分支特定的连接详细信息](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fji79akuf193gtv94yaag.png)

现在，您可以使用 `dev` 分支进行本地开发和测试，并使用 `main` 分支进行生产。这有助于将数据分开，并确保一个分支中的更改不会影响其他分支。

## 总结

在本文中，我们使用 Spring Boot、Neon Postgres 和 Azure App Service 构建了一个 CRUD 应用程序。

我们探讨了如何设置 Neon Postgres 数据库，使用 Spring Boot 构建一个基本的 CRUD 应用程序，将应用程序部署到 Azure App Service 上，并为应用程序和数据库配置自动缩放。

我们还了解了 Neon Postgres 中的数据库分支功能如何帮助您为不同环境和目的创建数据库分支。

[1]: https://neon.tech/
[2]: https://azure.microsoft.com/en-us/products/app-service
[3]: #what-is-neon-postgres
[4]: #how-to-set-up-the-database
[5]: #create-the-database
[6]: #how-to-build-the-spring-boot-crud-app
[7]: #create-an-entity-class
[8]: #create-a-repository
[9]: #create-a-rest-controller
[10]: #configure-the-database
[11]: #how-to-deploy-on-azure-app-service
[12]: #create-a-new-web-app
[13]: #deploy-the-application
[14]: #access-the-application
[15]: #how-to-set-up-autoscaling
[16]: #autoscaling-in-azure
[17]: #autoscaling-in-neon
[18]: #how-to-configure-database-branches-in-neon
[19]: #summary
[20]: https://console.neon.tech/signup
[21]: https://neon.tech/pricing
[22]: https://start.spring.io/
[23]: https://portal.azure.com/
[24]: https://learn.microsoft.com/en-us/azure/azure-functions/functions-premium-plan?tabs=portal#plan-and-sku-settings
[25]: https://neon.tech/docs/introduction/autoscaling
[26]: https://neon.tech/docs/introduction/autoscaling

