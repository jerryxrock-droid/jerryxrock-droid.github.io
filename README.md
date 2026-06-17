# Jerry Xie · Personal Site

个人求职名片网站，目标是 **AI PM 转型求职**。

🌐 上线后访问：https://jerryxrock-droid.github.io

## 技术栈

- **静态站点生成**：Jekyll 4
- **主题**：[Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes)（gem-based）
- **部署**：GitHub Pages
- **费用**：¥0（完全免费）

## 本地开发

```bash
bundle install
bundle exec jekyll serve --livereload
# 访问 http://localhost:4000
```

## 目录结构

```
├── _config.yml          # 站点配置
├── _data/navigation.yml # 导航菜单
├── _pages/              # 单页（about / projects / blog / contact）
├── _posts/              # 博客文章（Markdown）
├── _projects/           # 项目案例（collection）
├── assets/images/       # 图片资源
└── index.html           # 首页 Hero（splash layout）
```

## 维护说明

- **改内容**：直接编辑 Markdown 文件，commit + push
- **改导航**：编辑 `_data/navigation.yml`
- **改主题色**：编辑 `_config.yml` 的 `minimal_mistakes_skin`（dark / light / air / aqua / contrast）
- **加新博客**：在 `_posts/` 创建 `YYYY-MM-DD-title.md`

## 内容占位

待 Jerry 提供后补全：
- [ ] 头像 + 微信二维码
- [ ] Cariad / 上汽大众 / 福特 详细项目数据
- [ ] AI PM 面试题库博客
- [ ] LinkedIn URL 验证
