```markdown
---
title: 如何使用 Google Sheets 和 React 构建一个基础的 CMS
date: 2024-08-12T02:38:08.653Z
author: Marco Venturi
authorURL: https://www.freecodecamp.org/news/author/marco-venturi/
originalURL: https://www.freecodecamp.org/news/how-to-build-a-basic-cms-with-google-sheets-and-reactjs/
translator: ""
reviewer: ""
---

在当今的数字环境中，创建一个既经济实惠又易于维护的内容管理系统 (CMS) 可能会很困难，特别是当你在紧张的预算下运营时。

<!-- more -->

本教程将向你展示一种利用 Google Sheets 作为临时数据库，并用 React 构建前端的解决方案。从而让你有效地绕过对专用服务器或传统数据库系统的需求。

这种方法不仅减少了与网页开发相关的开销成本，还简化了内容更新和管理。如果你想在没有大量投资的情况下启动自己的简单 CMS，这是一个理想的解决方案。

这种解决方案适用于职业初期的自由职业者和那些无法在网站上投入大量资金的客户。

## 为什么选择 Google Sheets？

选择 Google Sheets 作为你的 CMS 的基础，归结于它的简单性、灵活性和成本效益。

传统的网页开发需要一个后端服务器来处理数据，一个数据库来存储信息，以及一个前端来显示内容。但每一层都增加了复杂性和成本。

而 Google Sheets 作为一个高度可访问且直观的界面，消除了对服务器和数据库的需求。它让你的用户能够实时更新内容，就像任何 CMS 一样，但没有通常的设置和维护成本。这使得它成为个人、小企业或任何希望快速部署网页应用且费用最少的人的一个绝佳选择。

## 入门指南

在深入代码之前，确保你在系统上已经安装了 Node.js 和 npm。这些工具将允许我们创建一个 React 应用并管理其依赖。

现在让我们从 Google Sheets 开始。

### 第一步：设置你的 Google Sheets

1.  进入你的 Google Sheets
2.  打开你想使用的表格或创建一个新表格
3.  点击菜单中的 `扩展` 
4.  然后点击 `Apps Script`

在 Apps Script 编辑器中，你可以编写脚本，将其作为你的终端点。以下是一个将 Google Sheet 内容以 JSON 格式返回的脚本：

```javascript
function convertRangeToJson(data) {
  var jsonArray = [];

  // 检查数据是否为空或没有足够的行用于标题和至少一行数据
  if (!data || data.length < 2) {
    // 根据需要返回空数组或有意义的信息
    return jsonArray; // 或者返回 'No data available';
  }

  var headers = data[0];
  for (var i = 1, length = data.length; i < length; i++) {
    var row = data[i];
    var record = {};

    for (var j = 0; j < row.length; j++) {
      record[headers[j]] = row[j];
    }

    jsonArray.push(record);
  }

  return jsonArray;
}
```

然后：

1.  点击 `文件` > `保存`，并为你的项目命名
2.  点击 `部署` > `新部署`
3.  点击 `选择类型` 并选择 `网页应用`
4.  填写你的部署详细信息。在 `执行为` 下，选择脚本应作为你的帐户执行还是作为访问网页应用的用户执行。在 `谁有访问权` 下，选择谁可以访问你的网页应用。
5.  点击 `部署`

你可能会被要求授权脚本访问你的 Google Sheets。按照提示操作。

部署后，你将获得一个用于网页应用的网址。这是你的 API 终端。

为了让你了解目前的进展，以下是你的表格结构：

![Schermata-2024-03-04-alle-16.49.37](https://www.freecodecamp.org/news/content/images/2024/03/Schermata-2024-03-04-alle-16.49.37.png)

你的表格当前应当的样子

这是你调用终端点时得到的 JSON:

![postman_I](https://www.freecodecamp.org/news/content/images/2024/03/postman_I.png)

JSON

### 第二步：创建你的 React 应用

准备好 Google Sheets API 后，是时候创建一个 React 应用了，这个应用将获取并显示这些数据。

首先，创建一个 React 应用。在你的终端中运行以下命令来创建一个新的 React 应用：

```bash
npx create-react-app google-sheets-cards
cd google-sheets-cards
npm start
```

你也可以[使用现代构建工具如 Vite][1] 来实现这个目的，因为 CRA 已不再是构建 React 应用的推荐方式。

接下来，创建卡片组件。在 `src` 目录下，创建一个名为 `Card.js` 的文件。这个组件将负责显示每个数据记录：

```jsx
// src/Card.js
function Card({ title, content }) {
  return (
    <div className="card">
      <h1>{title}</h1>
      <p>{content}</p>
    </div>
  );
}

export default Card;
```

现在是时候在 App.js 中获取并显示你的数据了。修改 `App.js` 文件，包含从你的 Google Sheets API 获取数据的逻辑，并使用 Card 组件来显示这些数据：

```jsx
// src/App.js
import React, { useEffect, useState } from 'react';
import Card from './Card';
import './App.css'; // 确保在 App.css 中创建一些基本的卡片样式
```

```markdown
useEffect(() => {
    fetch('YOUR_ENDPOINT_URL') // 用您的实际端点 URL 替换
      .then(response => response.json())
      .then(data => setData(data))
      .catch(error => console.error('获取数据时出错:', error));
  }, []);

  return (
    <div className="App">
      <h1>来自谷歌表格的数据</h1>
      <div className="cards-container">
        {data.map((item, index) => (
          <Card key={index} title={item.Title} content={item.Content} />
        ))}
      </div>
    </div>
  );
}

export default App;
```

接下来，您可以为卡片添加样式。在 `App.css` 中添加以下 CSS 进行基础卡片样式设计：

```css
.card {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  margin: 10px;
  padding: 10px;
  display: inline-block;
  background: #f9f9f9;
}

.cards-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
```

### 步骤 3: 运行您的 React 应用

设置完毕后，您现在可以运行您的 React 应用，并在浏览器中查看来自谷歌表格的数据。按以下步骤操作：

首先，启动 React 应用。在终端中，导航到您的 React 应用的根目录（如果您尚未在该目录）。运行以下命令以启动开发服务器：

```bash
npm start
```

该命令会编译您的 React 应用并在您的默认网页浏览器中打开。您应该会看到一个标题为"Data from Google Sheets"的网页，下面是一系列卡片，每个卡片显示从您的谷歌表格数据获取的标题和内容。

实际上，我们得到了以下结果：

![Schermata-2024-03-04-alle-16.52.22](https://www.freecodecamp.org/news/content/images/2024/03/Schermata-2024-03-04-alle-16.52.22.png)

屏幕上显示了来自谷歌表格的数据及卡片 1、卡片 2 和卡片 3

现在您可以查看您的数据。页面上的每个卡片对应于谷歌表格中的一行，标题和内容字段按照您的 Card 组件规定显示。如果您对谷歌表格数据进行了任何更新，可以刷新网页以立即查看更改。

您可以将您的 React 应用部署到网上的众多服务之一，如 Github Actions 或 Netlify。这是一种简单高效的方法，以显著的性能免费托管您的前端应用。

## 结论

恭喜您！您已经创建了一个动态 Web 应用，能从谷歌表格获取数据并用 React 显示。

这种方法提供了一种灵活、简单的方式来管理应用的内容，无需后端服务器或数据库。

谷歌表格作为管理数据的一个可访问和协作的工具，而 React 允许您构建响应式和交互式用户界面。两者结合提供了一个强大的方案，用于创建可以快速更新和轻松维护的 Web 应用。

---

![Marco Venturi](https://www.freecodecamp.org/news/content/images/size/w60/2022/02/io.jpeg)

我是 Marco, 我热爱自动化。我从使过程更高效中获取乐趣。当我不沉浸在技术中时，您可以发现我探索新目的地。

---

如果这篇文章对您有帮助，请分享。

免费学编程。freeCodeCamp 的开源课程已经帮助超过 40,000 人找到开发者工作。 [开始学习][2]

[1]: https://www.freecodecamp.org/news/get-started-with-vite/
[2]: https://www.freecodecamp.org/learn/
```

