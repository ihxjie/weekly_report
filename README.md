# Weekly Report

## 这个项目是如何工作的
这个项目主要使用了 [OpenAI GPT-3.5 Turbo API](https://platform.openai.com/) 和 [Vercel Edge functions](https://vercel.com/features/edge-functions)。它根据用户输入构建一个 Prompt，通过 Vercel Edge 函数将其发送到 OpenAI GPT-3.5 Turbo API，然后将响应流传回应用程序。

## 在本地运行

**[OpenAI API](api.openai.com) 的域名若无法访问（本地先ping一下），可以通过Github提供的CodeSpaces进行调试**

1. 在[OpenAI](https://platform.openai.com/) 注册一个账号，拿到 API key。
2. 克隆这个仓库到本地，将.env.example重命名为.env，把API key放到里面。
3. 确保你本地的 npm 命令生效，执行以下命令
```bash
npm install
npm run dev
```
打开 `http://localhost:3000`


## 线上一键部署

用 [Vercel](https://vercel.com?utm_source=github&utm_medium=readme&utm_campaign=vercel-examples) 一键部署:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ihxjie/weekly_report&env=OPENAI_API_KEY&project-name=weekly_report&repo-name=weekly_report)

环境变量如下所示：
```
OPENAI_API_KEY=xxxxx
```

## 来源
分支来自于[guaguaguaxia/weekly_report](https://github.com/guaguaguaxia/weekly_report)同名项目
