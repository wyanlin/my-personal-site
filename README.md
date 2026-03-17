# 个人网站

一个简洁美观的个人博客网站，用于发布文章和生活感悟。

## 特性

- ✨ 简洁美观的设计风格
- 📝 支持文章列表和文章详情页
- 👤 包含关于页面
- 📱 响应式设计，适配手机和电脑
- ➕ 易于后续添加新文章
- ☁️ 免费托管在GitHub Pages

## 技术栈

- HTML5
- CSS3 (Flexbox/Grid)
- JavaScript (ES6+)
- Google Fonts (Inter字体)

## 项目结构

```
personal-website/
├── index.html          # 首页
├── about.html          # 关于页面
├── posts.html          # 文章列表页面
├── post/               # 文章详情页面
│   ├── first-post.html
│   └── second-post.html
├── css/
│   └── style.css       # 样式文件
├── js/
│   └── main.js         # JavaScript文件
├── posts/              # Markdown源文件（用于参考）
│   ├── first-post.md
│   └── second-post.md
├── .gitignore
└── README.md
```

## 如何添加新文章

1. 在 `posts/` 目录下创建新的Markdown文件作为草稿
2. 在 `post/` 目录下创建对应的HTML文件
3. 在 `index.html` 和 `posts.html` 中添加新的文章卡片链接

### 新文章HTML模板

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>文章标题 - 个人网站</title>
    <link rel="stylesheet" href="../css/style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
</head>
<body>
    <header class="header">
        <div class="container nav-container">
            <a href="../index.html" class="logo">我的博客</a>
            <ul class="nav-links">
                <li><a href="../index.html">首页</a></li>
                <li><a href="../about.html">关于</a></li>
            </ul>
        </div>
    </header>

    <main class="main-content">
        <div class="container">
            <article class="article-content">
                <header class="article-header">
                    <h1 class="article-title">文章标题</h1>
                    <div class="article-meta">发布日期：YYYY年MM月DD日</div>
                </header>
                
                <!-- 文章内容 -->
                <p>你的文章内容...</p>
            </article>
        </div>
    </main>

    <footer class="footer">
        <div class="container">
            <p>&copy; 2026 我的个人网站. 保留所有权利.</p>
        </div>
    </footer>

    <script src="../js/main.js"></script>
</body>
</html>
```

## 部署到GitHub Pages

1. 在GitHub上创建一个新的仓库（例如：`your-username.github.io`）
2. 将本地代码推送到该仓库：
   ```bash
   git remote add origin https://github.com/your-username/your-username.github.io.git
   git push -u origin master
   ```
3. 访问 `https://your-username.github.io` 查看你的网站

## 自定义

- 修改 `index.html` 中的网站标题和描述
- 在 `css/style.css` 中调整颜色主题
- 在 `about.html` 中更新个人信息

## 许可证

MIT License