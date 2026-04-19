# 贰只晓鱼的技术博客

基于GitHub Pages + Jekyll构建的个人技术博客。

## 🎯 博客主题

分享以下内容：
- OpenClaw配置和使用教程
- 自动化工具开发经验
- 技术问题解决方案
- 开源项目介绍

## 🚀 快速开始

### 本地开发
```bash
# 安装Jekyll
gem install bundler jekyll

# 克隆仓库
git clone https://github.com/2026erzhixiaoyu/blog.git
cd blog

# 安装依赖
bundle install

# 启动本地服务器
bundle exec jekyll serve
```

### 访问博客
- 在线地址：https://2026erzhixiaoyu.github.io/blog/
- GitHub仓库：https://github.com/2026erzhixiaoyu/blog

## 📁 目录结构

```
blog/
├── _config.yml          # 配置文件
├── _layouts/            # 布局文件
├── _includes/           # 包含文件
├── _posts/              # 博客文章
├── _pages/              # 静态页面
├── assets/              # 资源文件
├── .github/workflows/   # GitHub Actions
└── README.md            # 说明文件
```

## 📝 写作指南

### 新建文章
在 `_posts` 目录下创建Markdown文件，文件名格式：
```
YYYY-MM-DD-title.md
```

### 文章Front Matter
```yaml
---
layout: default
title: "文章标题"
date: YYYY-MM-DD
categories: [分类1, 分类2]
tags: [标签1, 标签2]
excerpt: "文章摘要"
---
```

## 🔧 技术栈

- **静态网站生成器**: Jekyll
- **部署平台**: GitHub Pages
- **样式**: 自定义CSS
- **图标**: Font Awesome
- **代码高亮**: Rouge

## 🤝 贡献

欢迎提交Issue和Pull Request！

### 贡献指南
1. Fork本仓库
2. 创建功能分支
3. 提交更改
4. 推送到分支
5. 创建Pull Request

## 📄 许可证

本博客内容采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证。

## 📞 联系

- 作者：贰只晓鱼
- 邮箱：3962235311@qq.com
- 微信：XY18321979968（请备注OpenClaw）
- GitHub：[@2026erzhixiaoyu](https://github.com/2026erzhixiaoyu)

## 🙏 致谢

感谢以下项目：
- [Jekyll](https://jekyllrb.com/)
- [GitHub Pages](https://pages.github.com/)
- [Font Awesome](https://fontawesome.com/)
- 所有开源贡献者
