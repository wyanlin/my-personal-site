# 部署到GitHub Pages的步骤

## 1. 创建GitHub仓库
1. 登录到您的GitHub账户
2. 点击右上角的"+"号，选择"New repository"
3. 仓库名称建议使用 `username.github.io` 格式（将username替换为您的GitHub用户名）
4. 选择"Public"（公开）
5. 不要初始化README、.gitignore或license文件
6. 点击"Create repository"

## 2. 推送代码到GitHub
在您的本地机器上执行以下命令：

```bash
# 克隆您刚刚创建的仓库（替换your-username为您的GitHub用户名）
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io

# 将我们创建的文件复制到仓库目录中
# （假设personal-website文件夹与仓库在同一目录）
cp -r ../personal-website/* .

# 添加、提交并推送
git add .
git commit -m "Initial commit: Personal website with articles and about page"
git push origin main
```

## 3. 访问您的网站
推送完成后，您的网站将在以下URL可用：
`https://your-username.github.io`

## 替代部署选项

### Vercel部署
1. 访问 [Vercel](https://vercel.com/)
2. 使用GitHub账户登录
3. 点击"New Project"
4. 选择您的个人网站仓库
5. 保持默认设置，点击"Deploy"
6. Vercel会自动为您分配一个域名

### Netlify部署
1. 访问 [Netlify](https://netlify.com/)
2. 使用GitHub账户登录
3. 点击"New site from Git"
4. 选择您的GitHub仓库
5. 保持默认构建设置（因为这是静态网站，不需要构建步骤）
6. 点击"Deploy site"

## 后续添加新文章

要添加新文章，只需：

1. 在 `posts/` 目录中创建新的Markdown文件（如 `third-post.md`）
2. 在 `post/` 目录中创建对应的HTML文件（如 `third-post.html`）
3. 更新 `index.html` 和 `posts.html` 中的文章列表
4. 提交并推送更改

或者，您可以考虑使用静态站点生成器（如Jekyll、Hugo或Eleventy）来自动化这个过程。