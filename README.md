# 个人网站

这是一个简洁美观的个人博客网站，用于发布文章和生活感悟。

## 功能特性

- ✨ 简洁美观的设计风格
- 📝 支持文章列表和文章详情页
- 👤 包含关于页面
- 📱 响应式设计，适配手机和电脑
- ➕ 易于后续添加新文章
- ☁️ 部署到免费托管平台

## 技术栈

- HTML5
- CSS3 (现代CSS特性，Flexbox, Grid)
- JavaScript (轻量级交互)
- Google Fonts (Inter字体)

## 如何添加新文章

1. 在 `posts/` 目录下创建新的Markdown文件（用于内容管理）
2. 在 `post/` 目录下创建对应的HTML文件
3. 在 `index.html` 和 `posts.html` 中添加文章链接

## 部署说明

这个网站可以直接部署到以下免费托管平台：

### GitHub Pages
1. 创建一个新的GitHub仓库
2. 将所有文件推送到仓库
3. 在仓库设置中启用GitHub Pages（选择main分支）

### Vercel
1. 导入GitHub仓库到Vercel
2. 自动部署，无需额外配置

### Netlify
1. 导入GitHub仓库到Netlify
2. 自动部署，支持自定义域名

## 文件结构

```
personal-website/
├── index.html          # 首页
├── about.html          # 关于页面
├── posts.html          # 文章列表页面
├── css/
│   └── style.css       # 样式文件
├── js/
│   └── main.js         # JavaScript文件
├── post/               # 文章详情页面
│   ├── first-post.html
│   └── second-post.html
└── posts/              # Markdown源文件（便于内容管理）
    ├── first-post.md
    └── second-post.md
```

## 许可证

MIT License