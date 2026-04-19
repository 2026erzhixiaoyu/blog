# 博客部署指南

## 部署状态

### 当前状态
- ✅ 博客结构已创建
- ✅ 配置文件已设置
- ✅ 第一篇文章已添加
- ✅ GitHub Actions工作流已配置
- ⏳ 等待推送到GitHub

### 部署步骤

#### 步骤1：初始化Git仓库
```bash
cd /root/.openclaw/workspace/blog
git init
git add .
git commit -m "初始提交：创建个人博客"
```

#### 步骤2：添加远程仓库
```bash
git remote add origin https://github.com/2026erzhixiaoyu/blog.git
```

#### 步骤3：推送到GitHub
```bash
git push -u origin main
```

#### 步骤4：启用GitHub Pages
1. 访问 https://github.com/2026erzhixiaoyu/blog/settings/pages
2. 选择 Source: GitHub Actions
3. 保存设置

#### 步骤5：等待部署完成
GitHub Actions会自动构建并部署到GitHub Pages。

## 访问地址

部署完成后，博客可通过以下地址访问：
- https://2026erzhixiaoyu.github.io/blog/

## 后续维护

### 添加新文章
1. 在 `_posts` 目录创建新文章
2. 使用正确的文件名格式：`YYYY-MM-DD-title.md`
3. 添加Front Matter配置
4. 提交并推送更改

### 更新配置
修改 `_config.yml` 文件后需要重新部署。

### 自定义样式
修改 `_layouts/default.html` 中的CSS样式。

## 问题排查

### 常见问题

#### 1. 页面无法访问
- 检查GitHub Pages设置
- 查看GitHub Actions构建日志
- 确认仓库是否为公开

#### 2. 样式加载失败
- 检查CSS路径
- 确认网络连接
- 清除浏览器缓存

#### 3. 文章不显示
- 检查Front Matter格式
- 确认文件名格式
- 查看构建日志中的错误

#### 4. 本地无法运行
- 检查Ruby和Jekyll版本
- 确认依赖已安装
- 查看错误信息

## 性能优化

### 图片优化
- 使用压缩后的图片
- 添加alt文本
- 使用合适的格式（WebP优先）

### 代码优化
- 压缩CSS和JavaScript
- 使用CDN加载资源
- 启用浏览器缓存

### SEO优化
- 添加meta描述
- 使用语义化标签
- 创建sitemap

## 安全考虑

### 内容安全
- 不泄露敏感信息
- 使用HTTPS
- 定期备份内容

### 账号安全
- 使用强密码
- 启用双因素认证
- 定期检查访问日志

## 扩展功能

### 可添加的功能
1. 评论系统（如Giscus）
2. 搜索功能
3. 文章分类页面
4. 标签云
5. 阅读统计

### 集成服务
1. Google Analytics
2. 百度统计
3. 邮件订阅
4. RSS订阅

## 联系方式

如有部署问题，请联系：
- 飞书：贰只晓鱼
- 微信：XY18321979968
- 邮箱：3962235311@qq.com
