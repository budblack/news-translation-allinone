---
title: How to Develop a CRUD App with Spring Boot, Neon Postgres, and Azure App
  Service
date: 2024-07-28T07:47:06.061Z
author: Abhinav Pandey
authorURL: https://www.freecodecamp.org/news/author/abhinav-pandey/
OriginalURL: https://www.freecodecamp.org/news/build-a-crud-app-spring-boot-neon-postgres/
Proofreader: ""

---

In this article, we'll explore how to develop a CRUD (Create, Read, Update, Delete) application using Spring Boot and [Neon Postgres][1].

<!-- more -->

We'll also deploy the application on [Azure App Service][2] and make it production-ready by setting up features like autoscaling and multiple environments.

You'll learn how Neon Postgres can make your development and deployment processes easier along the way.

## Here's what we'll cover:

-   Setting up a Neon Postgres database and exploring its features
-   Building a CRUD application using Spring Boot and deploying the application on Azure App Service
-   Why Neon is a good fit for infrastructure that auto-scales
-   Database branching in Neon Postgres and how it can ease the development workflow

## Prerequisites

-   Working knowledge of Java, Maven, and Spring Boot
-   Basics of SQL databases
-   Understanding of serverless and cloud services
-   Familiarity with testing and deployment processes

## Table of Contents

-   [What is Neon Postgres?][3]
-   [How to Set Up the Database][4]
    -   [Create the Database][5]
-   [How to Build the Spring Boot CRUD App][6]
    -   [Create an Entity Class][7]
    -   [Create a Repository][8]
    -   [Create a REST Controller][9]
    -   [Configure the Database][10]
-   [How to Deploy on Azure App Service][11]
    -   [Create a New Web App][12]
    -   [Deploy the Application][13]
    -   [Access the Application][14]
-   [How to Set Up Autoscaling][15]
    -   [Autoscaling in Azure][16]
    -   [Autoscaling in Neon][17]
-   [How to Configure Database Branches in Neon][18]
-   [Summary][19]

## What is Neon Postgres?

Neon is a fully managed serverless Postgres database platform. It offers features such as high availability, automatic backups, and scaling options to handle varying traffic levels.

Neon is designed to be cost-efficient and developer-friendly, and it focuses on providing a seamless experience for developers.

In addition to the standard Postgres features, it provides capabilities like database branching, allowing you to create Git-like branches of the database for different purposes.

## How to Set Up the Database

To begin with, let's explore how you can set up a Neon database for your application.

Firstly, you'll need to [create an account][20] on the Neon website. It doesn't require a credit card to sign up, and you're automatically set up with the free tier to get started.

Here's a [pricing and features comparison][21] of Neon plans:

![A screenshot of pricing plans in Neon listing down free and paid features](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Finxumg46sf92ffre6l2q.png)

Neon pricing plans

In the free tier, we get 0.5 GB of storage with basic computing which is enough for playing around with the database and building small applications.

### Create the Database

Once you've signed up, you can access the dashboard and create a new project.

Star by filling in the project name, region, and Postgres version options. In addition to this, we can choose two additional options:

-   **compute size** – You can choose a min and max compute size for the database. This is useful for autoscaling the database based on the load.
-   **suspend time** – You can set a time after which the database will be suspended if not being used. This is useful for saving costs when the database is not being used.

![Form with specifications required when creating a database](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fggwuvqtb8ydl3mxd1dak.png)

Creating a database project in Neon

Once you submit the form, Neon will create the database and provide the connection details.

![Neon Dashboard showing the project is ready. Also shows connection details.](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fwe2x5d81euphg2owgxhd.png)

Neon Dashboard

As you can see, the database was set up in 3.3 seconds (compared to hours of installing and setting up your own infrastructure). You can choose multiple ways to connect to the database. For this tutorial, select Java as your programming language and get the JDBC connection string.

## How to Build the Spring Boot CRUD App

Next, let's set up our CRUD application. We'll use Spring Boot, as it provides easy bootstrapping and configuration for building web applications.

We can use the [Spring Initializr][22] to generate a new Spring Boot project with the necessary dependencies:

-   Spring Web – for building web applications
-   Spring Data JPA – for working with databases using JPA
-   PostGres Driver – for connecting to the Postgres database

![Spring Initializer website form to select spring boot project specifications and dependencies](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Ffifv17tc5d3swothe3zf.png)

Creating a Spring Boot project using Spring Initializer

You can generate, download, and import the project into your favorite IDE.

### Create an Entity Class

Let's create an entity class to represent the data in the application. First, create a `User` class:

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

The entity name `users` is the name of the table you want to use in your database.

### Create a Repository

Next, create a repository interface to interact with the database. You'll extend the `JpaRepository` interface provided by Spring Data JPA:

```Java
@Repository
public interface UserRepository extends JpaRepository<User, Long> {
}
```

You need to annotate the interface with `@Repository` to mark it as a Spring bean. The `JpaRepository` interface provides methods for CRUD operations like `save`, `findAll`, `findById`, `delete`, and so on, so you don't need to write the queries manually.

You'll provide your entity class `User` and the type of the primary key `Long` as type arguments to the `JpaRepository` interface.

### Create a REST Controller

Finally, create a REST controller to handle the CRUD operations. You'll inject the `UserRepository` into the controller and implement the necessary endpoints:

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

Here are a few things to note:

-   You're using the `@RestController` annotation to mark the class as a controller that handles REST requests.
-   The `@RequestMapping` annotation specifies the base URL for the endpoints.
-   You're injecting the `UserRepository` into the controller using constructor injection.
-   Finally, you're implementing your API endpoints for CRUD operations using the `@GetMapping`, `@PostMapping`, `@PutMapping`, and `@DeleteMapping` annotations.

### Configure the Database

To connect your Spring Boot application to the Neon Postgres database, you need to configure the database URL, username, and password in the `application.properties` file:

```
spring.datasource.url=jdbc:postgresql://<db-url>/<db-name>?sslmode=require
spring.datasource.username=<username>
spring.datasource.password=<password>
spring.jpa.hibernate.ddl-auto=update
```

Here, you configured the database URL, username, and password provided by Neon when you created the database. The `spring.jpa.hibernate.ddl-auto=update` property tells Spring Boot to automatically create the necessary tables or columns based on the entity classes when the application starts.

## How to Deploy on Azure App Service

Now that your Spring Boot application is ready, it's time to deploy it on Azure App Service.

### Create a New Web App

To deploy your Spring Boot application on Azure App Service, you'll first create a new `Web App`. You can do this through the Azure portal by following these steps:

-   Log in to the [Azure portal][23].
-   Click on the `Create a resource` button.
-   Search for `Web App` and select the `Create` option.
-   Fill in the necessary details like resource group, app name, runtime stack, and region.
-   Click the `Review + create` button.

![Form for creating a web app in Azure](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Flf2kmh12t8eucd1qa1pg.png)

Creating a Web App in Azure

### Deploy the Application

The Web App takes a couple of minutes to create. Once done, you can deploy your Spring Boot application to Azure App Service.

One of the easiest ways to deploy is to package your Spring Boot application as a JAR file and deploy it to Azure App Service using the Azure CLI.

To do this, run the below commands:

```
mvn package
az webapp deploy --src-path neon-demo-0.0.1-SNAPSHOT.jar --resource-group learn-ba1a439c-71ca-4cab-9bb1-f5b1331bab04 --name neon-app
```

Here, you're packaging your Spring Boot application using Maven and deploying the JAR file to Azure App Service using the Azure CLI. You've provided the path to the JAR file, the resource group, and the app name you previously configured.

### Access the Application

Once the deployment is complete, you can access your Spring Boot application on Azure App Service by navigating to the URL of the Web App. Your app is available at neon-app.azurewebsites.net

Let's use \_curl \_to test the endpoints.

#### Create a User

```
curl -X POST -d '{"name":"John Doe","email":"john@gmail.com"}' https://neon-app.azurewebsites.net/users
```

Here you provide user data in JSON format to create a new user.

#### Get Users

You can also can test that the user was created by fetching all users:

```
curl -X GET https://neon-app.azurewebsites.net/users
```

## How to Set Up Autoscaling

A production application may experience varying levels of traffic, and it's important to scale the application dynamically based on the load.

Let's explore how you can autoscale your application when needed.

### Autoscaling in Azure

Azure App Service provides [autoscaling options][24] that let you automatically adjust the number of instances as needed.

You can configure autoscaling rules in the Azure portal by following these steps:

-   Navigate to the Web App in the Azure portal.
-   Click the `Scale out (App Service Plan)` option from the left menu.
-   Configure the autoscaling rules – you can choose predefined rules like traffic or create custom rules based on metrics like CPU usage, memory usage, or custom metrics.
-   Save.

Azure will automatically scale the application based on the configured rules.

### Autoscaling in Neon

Since your application is automatically scaled based on the load, you'll want to ensure that the database can handle the increased traffic.

Neon provides [autoscaling options][25] to scale the database dynamically based on the load. You can configure autoscaling rules in the Neon dashboard to ensure the database can handle the increased load.

Follow the below steps to configure autoscaling in Neon:

1.  Navigate to the Neon dashboard and select the database. Then select the branch to configure autoscaling.

![Neon project dashboard with branches section highlighted ](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fl6s84pqhk2avflpjbgrf.png)

Selecting a branch from Neon project dashboard

2\.  Click on the `Edit` button next to the `Compute` section. Configure the autoscaling rules based on metrics like CPU usage, memory usage, or custom metrics.

![Branch details view in Neon with edit button in the computes section highlighted](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Ffkn11nop1zz9xxbfamsr.png)

Branch details view in Neon

3\.  Configure the min-max compute size and Save. Neon will automatically scale the database based on the configured rules when needed.

![Form to enable autoscaling and select min and max size of the compute](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fdmuow8zvndz0dibv2kxt.png)

Setting up autoscaling for compute

Ensuring that both the application and the database can scale dynamically based on the load will help you handle varying levels of traffic efficiently.

## How to Configure Database Branches in Neon

In a typical development workflow, multiple databases may be used for different purposes like development, testing, and production.

Neon Postgres provides [database branching][26] to create multiple branches for different purposes. Each branch is an instance of the database that you can use independently.

This Git-like feature helps set up a copy of the database for different environments like development, staging, and production. It also helps preserve data for different versions of the application.

Let's explore how you can create and manage branches in Neon Postgres:

-   Navigate to the Neon dashboard and select the database.
-   In the `Branches` section, click on the `View All` button.
-   You can create a new branch from an existing one by clicking on the `Create Branch` button. You'll need to provide the branch name and what data to copy from the parent branch.

![Branches view with Create branch option visible ](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F9ncdgdrj32etd3gbqurf.png)

Create branch option

-   You can either copy all the data or copy until a point in time or a specific record. This is useful for multiple purposes like restoring data, creating a new environment, or testing new features.

![Creating a new branch from an existing branch](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fw7gchucru5qw294icqw3.png)

Creating a new branch

-   Neon will create a new branch of the database that can be used independently. You can find the URL, username, and password for the new branch in the dashboard. And this happens in real time without any downtime and delays.

![Branch-specific connection details ](https://media.dev.to/cdn-cgi/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fji79akuf193gtv94yaag.png)

Branch-specific connection details

Now you can use your `dev` branch for local development and testing, and the `main` branch for production. This helps in keeping the data separate and ensures that changes in one branch do not affect the other branches.

## Summary

In this article, we built a CRUD application using Spring Boot, Neon Postgres, and Azure App Service.

We explored how to set up the Neon Postgres database, build a basic CRUD application using Spring Boot, deploy the application on Azure App Service, and configure autoscaling for the application and the database.

We also learned about how the database branching feature in Neon Postgres helps you create branches of the database for different environments and purposes.

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