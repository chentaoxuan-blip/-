# 海龟汤 · 情境猜谜游戏

一个基于 AI 主持人的海龟汤推理游戏，内置 25 道精选谜题，支持单人和多人模式。

## 部署到 Vercel（3步完成）

### 方法一：拖拽部署（最简单）

1. 打开 [vercel.com](https://vercel.com) 并登录
2. 点击 **Add New → Project**
3. 选择 **"Deploy from file"** 或直接把这个文件夹拖进去
4. 点击 Deploy，等待约 30 秒，获得专属链接

### 方法二：GitHub + Vercel（推荐，方便后续更新）

```bash
# 1. 在 GitHub 创建新仓库，然后：
git init
git add .
git commit -m "初始化海龟汤游戏"
git remote add origin https://github.com/你的用户名/turtle-soup.git
git push -u origin main

# 2. 在 vercel.com 导入该 GitHub 仓库
# 3. 自动部署，每次 git push 后自动更新
```

## 功能说明

- **25 道内置谜题**：分为入门 / 中等 / 烧脑三档，涵盖日常、悬疑、温情三类
- **分类筛选**：支持按难度和主题过滤
- **AI 生成谜题**：点击"让 AI 随机生成"可实时创作新题（需要网络）
- **AI 主持人**：由 Claude 担任主持人，严格按照规则只回答是/否/部分相关/无关
- **多人模式**：生成房间码，适合多人围坐一起玩

## 本地运行

直接用浏览器打开 `index.html` 即可，无需任何构建步骤。

## 技术栈

- 纯 HTML + CSS + JavaScript，零依赖
- 调用 Anthropic API（Claude Sonnet 4.6）驱动 AI 主持人
- 静态文件，可部署到任何托管平台
