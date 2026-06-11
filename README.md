# 问对设计 — 公司官网

现代简约风格的设计工作室官网，纯静态 HTML/CSS/JS，无需构建工具。

## 页面结构

| 文件 | 页面 |
|------|------|
| `index.html` | 首页（Hero、服务概览、精选案例） |
| `about.html` | 关于我们（理念、团队） |
| `services.html` | 服务（服务详情、工作流程） |
| `work.html` | 案例作品集 |
| `contact.html` | 联系我们（联系方式、表单） |
| `css/style.css` | 全站样式 |
| `js/main.js` | 移动端菜单、滚动动效 |

## 本地预览

直接双击 `index.html` 即可在浏览器打开。

## 上传到 GitHub 并发布（GitHub Pages）

### 第一步：创建 GitHub 仓库

1. 登录 [github.com](https://github.com)，点击右上角 **+** → **New repository**
2. 仓库名填写如 `company-website`（或 `你的用户名.github.io`，这样网址更短）
3. 选择 **Public**，**不要**勾选 "Add a README"，点击 **Create repository**

### 第二步：上传代码

在本文件夹中打开终端（Windows：文件夹空白处右键 → "在终端中打开"），依次执行：

```bash
git init
git add .
git commit -m "公司官网首版"
git branch -M main
git remote add origin https://github.com/你的用户名/company-website.git
git push -u origin main
```

> 没装 Git？先从 [git-scm.com](https://git-scm.com/download/win) 下载安装。
> 不想用命令行？在仓库页面点 **uploading an existing file**，把本文件夹所有文件拖进去上传即可。

### 第三步：开启 GitHub Pages

1. 进入仓库 → **Settings** → 左侧 **Pages**
2. **Source** 选择 `Deploy from a branch`，Branch 选 `main` / `(root)`，点 **Save**
3. 等待约 1 分钟，页面顶部会显示网址：
   `https://你的用户名.github.io/company-website/`

### 后续更新网站

修改文件后执行：

```bash
git add .
git commit -m "更新内容说明"
git push
```

推送后 GitHub Pages 会在一两分钟内自动更新。

## 自定义内容

- **公司信息**：搜索替换各 HTML 中的"问对设计"、邮箱、电话、地址
- **配色**：修改 `css/style.css` 顶部 `:root` 中的 `--accent` 等变量
- **案例图片**：目前用渐变色占位（`.work-thumb`），可替换为 `<img>` 真实图片
