# Jerry Xie · Personal Site

个人求职名片网站，目标是 **AI PM 转型求职**。

🌐 **线上地址**：https://jerryxrock-droid.github.io

## 技术栈

- **静态站点生成**：Jekyll 4
- **主题**：[Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes)
- **部署**：GitHub Pages + GitHub Actions
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
├── index.html           # 首页 Hero
├── about.md             # /about
├── projects.md          # /projects 列表
├── contact.md           # /contact
├── blog.md              # /blog 列表
├── 404.md               # 404 页
├── _posts/              # 博客文章（Markdown）
│   └── 2026-06-17-why-ai-pm-pivot.md
├── _projects/           # 项目案例（collection）
│   └── cariad-data-collection.md
├── _data/
│   └── navigation.yml   # 顶部导航
├── assets/images/       # 图片资源
└── .github/workflows/jekyll.yml
```

## 维护说明

- **改内容**：直接编辑 Markdown 文件 → `git add -A && git commit -m "..." && git push`
- **加博客**：在 `_posts/` 创建 `YYYY-MM-DD-title.md`，frontmatter 加 `permalink: /blog/标题/`
- **加项目**：在 `_projects/` 创建 `name.md`
- **改主题色**：编辑 `_config.yml` 的 `minimal_mistakes_skin`

---

## 📋 待补资料清单（影响求职效果）

按优先级排。**任何一项填上后网站会立即更有说服力**。

### 🔴 P0：核心展示（缺了影响 HR 第一印象）

- [ ] **微信二维码** → 保存到 `assets/images/qrcode-wechat.png`
- [ ] **头像照片** → 保存到 `assets/images/avatar.png`（300x300 圆角）
- [ ] **LinkedIn URL** → 更新 `contact.md`
- [ ] **Cariad 项目具体内容**（在 `_projects/cariad-data-collection.md`）：
  - 2-3 个具体项目名 + 关键数据指标
  - 跨部门协调的具体挑战与解决
  - 复盘（做对/做错）

### 🟡 P1：经历细节（影响猎头判断深度）

- [ ] **精确时间线**（在 `about.md`）：
  - 泛亚、福特、上汽大众 各自的精确起止时间
  - 各阶段的汇报对象 / 团队规模
- [ ] **上汽大众 / 福特的关键项目 + 成果**（在 `projects.md`）
- [ ] **薪资范围**（在 `contact.md`，可选）

### 🟢 P2：锦上添花（求职季开始后优化）

- [ ] **AI PM 面试题库博客**（按 5 模块拆解）
- [ ] **Xuanjing 项目 README 完善**
- [ ] **FitEat_J / daily_stock_analysis 项目截图**
- [ ] **公众号 / 掘金 / 知乎 同步输出**

### ⚙️ P3：长期优化

- [ ] **自定义域名 sheldonxie.com**（求职季开始时再决定）
- [ ] **Lighthouse 性能跑分 + 优化**
- [ ] **暗色/亮色主题切换**
- [ ] **联系表单后端**（目前只展示联系方式）

---

## 🚀 部署流程

1. 改完本地文件
2. `git add -A`
3. `git commit -m "..."`
4. `git push origin main`
5. GitHub Actions 自动 build + 部署
6. 1-2 分钟后刷新 `https://jerryxrock-droid.github.io` 即可看到

## 历史踩坑（重要，避免重蹈）

| # | 问题 | 修复 |
|---|------|------|
| 1 | GitHub Pages 找不到 minimal-mistakes 主题 | Gemfile 加 `gem "minimal-mistakes-jekyll"`，`_config.yml` 写 `theme: minimal-mistakes-jekyll`（带 -jekyll 后缀） |
| 2 | 4.x 主题用 `include_cached` 需要 Jekyll 4 | 用 GitHub Actions build（`build_type: workflow`）而不是 Pages 内置 Jekyll build |
| 3 | `_pages/*.md` 404 | Jekyll 不输出未声明的 collection，移到根目录 |
| 4 | 博客 URL 包含 `/categories/` | frontmatter 加 `permalink: /blog/标题/` |
