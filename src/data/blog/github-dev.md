---
slug: github-dev
title: github-dev
author: lorilu
pubDatetime: 2026-03-18T15:33:05.569Z
description: github-dev
featured: true
draft: false
tags:
  - TEST
---



**GitHub Dev (`github.dev`) 是 GitHub 官方推出的网页版编辑器**。

它本质上是将 **VS Code** 完整地搬到了浏览器里。你可以直接在任何仓库页面按下键盘上的 **句号键 (`.`)**，它就会瞬间切换到这个编辑器模式。

对于你目前这种“被 TinaCMS 折腾坏了”的情况，GitHub Dev 可能是最适合你的“减法”方案：

### 为什么它比 CMS 更适合你？

1.  **官方原生支持**：由 GitHub 维护，账号通用，安全性最高。
2.  **零配置、零依赖**：你不需要在 `package.json` 里安装任何包，也不需要配置任何环境变量，更不会有 React 19 的兼容性问题。
3.  **环境一致性**：因为它就是 VS Code，你熟悉的快捷键、Markdown 预览、文件夹目录树都在，体验和你本地开发几乎一样。
4.  **即时构建**：你在网页版 VS Code 里修改并点击“提交（Commit）”后，Vercel 会立即感应到 GitHub 的变动并开始自动构建。

---

### 如何高效使用它管理博客？

既然你用的是 **AstroPaper**，你可以按照以下流程操作：

1.  **快速进入**：访问你的 GitHub 仓库页面，按下键盘的 `.` 键（或者把 URL 里的 `.com` 改成 `.dev`）。
2.  **创建博文**：在左侧文件树找到 `src/content/blog/`，右键新建文件（如 `my-new-post.md`）。
3.  **填写 Frontmatter**：
    > **小技巧**：你可以打开一篇旧文章，复制头部的 `title`, `pubDatetime` 等配置，改改内容即可。
4.  **实时预览**：点击右上角的“预览”图标（或者按下 `Ctrl+Shift+V`），可以直接看到 Markdown 渲染后的样子。
5.  **发布上线**：点击左侧侧边栏的 **“源代码管理”图标**（那个像分支的图标），输入提交信息（如 "feat: add new post"），点击 **"Commit & Push"**。

---

### 进阶：如果你想要更强大的“类 CMS”体验

如果你觉得手动复制 Frontmatter 麻烦，可以在 `.github` 目录下创建一个 **Issue Template** 或者使用 **VS Code Snippets**。

在 GitHub Dev 中，你可以配置自定义代码片段（Snippets）：
1.  按 `Ctrl+Shift+P`，搜索 `User Snippets`。
2.  选择 `markdown`。
3.  加入一个 `new-blog` 模板，以后输入 `blog` 就能一键生成带日期的标准头部。

---
 