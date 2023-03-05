# [Weekly Report](https://report.ihxjie.cn/zh)

简单描述工作内容，帮你生成完整周报

[![Weekly Report](./public/screenshot.jpg)](https://report.ihxjie.cn/zh)

## 这个项目是如何工作的
这个项目主要使用了 [OpenAI GPT-3.5 Turbo API](https://platform.openai.com/) 和 [Vercel Edge functions](https://vercel.com/features/edge-functions)。它根据用户输入构建一个 Prompt，通过 Vercel Edge 函数将其发送到 GPT-3 API，然后将响应流传回应用程序。

## 在本地运行

**OpenAI API 的域名 api.openai.com 现无法在大陆网络环境下访问，可以通过Github提供的CodeSpaces进行调试**

clone 此 repo，去 [OpenAI](https://beta.openai.com/account/api-keys) 注册一个账号，拿到 API key，放到 `.env` 文件。本地文件 `.env.example` 要改成 `.env`。


确保你本地的 npm 命令生效，执行以下命令
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
