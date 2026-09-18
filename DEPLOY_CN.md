# 发布到 GitHub Pages

## 方式一：网页上传（最简单）

1. 登录 GitHub，点击右上角 `+` → **New repository**。
2. Repository name 填写 `你的用户名.github.io`。例如 GitHub 用户名是 `on1262`，仓库名就是 `on1262.github.io`。
3. 选择 **Public**，点击 **Create repository**。
4. 解压网站压缩包，进入 `yutong-chen-academic` 文件夹。
5. 在空仓库页面点击 **uploading an existing file**，将该文件夹里的全部文件和文件夹拖入上传区域。注意：应直接看到 `index.html`，不要再套一层目录。
6. 在页面底部填写提交说明（例如 `Initial academic website`），点击 **Commit changes**。
7. 进入仓库 **Settings** → 左侧 **Pages**。
8. 在 **Build and deployment** 中，将 Source 设为 **Deploy from a branch**；Branch 选择 `main`，目录选择 `/ (root)`，然后 **Save**。
9. 等待约 1–5 分钟，访问 `https://你的用户名.github.io/`。

## 方式二：使用 Git 命令

在解压后的 `yutong-chen-academic` 目录中运行：

```bash
git init
git add .
git commit -m "Initial academic website"
git branch -M main
git remote add origin https://github.com/你的用户名/你的用户名.github.io.git
git push -u origin main
```

随后按方式一的第 7–9 步启用 GitHub Pages。

## 日后更新

- 修改个人简介或 News：编辑 `index.html`
- 修改论文：编辑 `publications.html`
- 修改研究项目：编辑 `research.html`
- 更新简历：用新 PDF 覆盖 `files/Yutong_Chen_CV.pdf`
- 更新头像：用新图片覆盖 `assets/images/profile.jpg`

每次改完后重新上传并提交，GitHub Pages 会自动更新网站。

## 常见问题

- **打开网站显示 404**：检查仓库名是否严格为 `用户名.github.io`，并确认 `index.html` 位于仓库根目录。
- **样式或图片丢失**：不要改变 `assets` 文件夹的层级，也不要只上传 HTML 文件。
- **发布后没有立即更新**：在仓库的 **Actions** 或 **Settings → Pages** 查看部署状态，并等待几分钟后强制刷新浏览器。
- **使用自定义域名**：先在 **Settings → Pages → Custom domain** 填写域名，再按照 GitHub 提示配置 DNS。
