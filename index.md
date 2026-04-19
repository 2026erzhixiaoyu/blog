---
layout: default
title: 首页
---

## 📚 最新文章

<ul class="post-list">
{% for post in site.posts limit:5 %}
  <li class="post-item">
    <h2 class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <div class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%Y年%m月%d日" }}
      </time>
      • {{ post.category | default: "未分类" }}
    </div>
    <div class="post-excerpt">
      {{ post.excerpt | strip_html | truncate: 200 }}
    </div>
    <a href="{{ post.url | relative_url }}" class="read-more">阅读全文 →</a>
  </li>
{% endfor %}
</ul>

{% if site.posts.size > 5 %}
<div style="text-align: center; margin-top: 2rem;">
  <a href="/archive" class="read-more">查看所有文章 →</a>
</div>
{% endif %}

## 🎯 服务项目

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1.5rem; margin-top: 2rem;">
  <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
    <h3 style="margin-bottom: 1rem;">OpenClaw配置指导</h3>
    <p>一对一配置指导，解决安装、配置、使用中的各种问题。</p>
  </div>
  
  <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
    <h3 style="margin-bottom: 1rem;">自动化工作流定制</h3>
    <p>根据需求定制自动化脚本和工作流，提高工作效率。</p>
  </div>
  
  <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
    <h3 style="margin-bottom: 1rem;">GitHub工具开发</h3>
    <p>开发实用的GitHub工具和自动化脚本。</p>
  </div>
  
  <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
    <h3 style="margin-bottom: 1rem;">企业级部署支持</h3>
    <p>为企业提供OpenClaw部署、定制和培训服务。</p>
  </div>
</div>

## 📊 开源项目

<div style="margin-top: 2rem;">
  <h3>GitHub项目</h3>
  <ul>
    <li><a href="https://github.com/2026erzhixiaoyu/openclaw-guides" target="_blank">OpenClaw配置指南</a> - 完整的OpenClaw配置教程</li>
    <li><a href="https://github.com/yourusername/github-sync-tool" target="_blank">GitHub同步工具</a> - 自动化文件同步工具</li>
  </ul>
</div>
