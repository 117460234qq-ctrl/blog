# Tiger Lin — 个人博客

深色优雅风格的个人博客，纯静态 HTML/CSS/JS。与公司网站同源设计语言，但更注重阅读体验：衬线标题、金色点缀、杂志式排版。

## 文件结构

| 文件 | 页面 |
|------|------|
| `index.html` | 首页（精选、最近文章、专栏、订阅） |
| `posts.html` | 文章归档 |
| `post.html` | 文章详情（示例文章，可复制此文件写新文章） |
| `about.html` | 关于我 |
| `blog.css` | 全站样式 |
| `blog.js` | 移动端菜单、滚动动效 |

## 写新文章

复制 `post.html` 改名（如 `post-2.html`），替换标题、日期和正文，再到 `index.html` 和 `posts.html` 的列表中加一条链接。

## 发布到 GitHub Pages

与公司网站相同：新建仓库（如 `blog`）→ 把本文件夹内所有文件拖拽上传 → Settings → Pages 开启 `main` 分支发布。网址将是 `https://你的用户名.github.io/blog/`。

## 自定义

- 配色在 `blog.css` 顶部 `:root`：`--gold` 是点缀色，`--bg` 是背景色
- 作者名搜索替换 "Tiger Lin"，邮箱替换 `hi@tigerlin.me`
- 订阅表单目前是演示用，可接入 Buttondown / Mailchimp 等服务
