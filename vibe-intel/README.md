# 🌐 Vibe Coding & AI 情报日报
> 每日追踪 vibe coding、agent engineering 市场动态  
> 网页版：https://xiajngsi.github.io/showcase/vibe-intel/

## 📅 历史报告
- [2026-03-16](reports/2026-03-16.md) · [HTML](reports/2026-03-16.html)
- [2026-03-15](reports/2026-03-15.md)
- [2026-03-14](reports/2026-03-14.md)
- [2026-03-13](reports/2026-03-13.md) · [HTML](reports/2026-03-13.html)

---

## 📋 HTML 同步规则

每期 Markdown 简报需同步发布为 HTML 文件，以支持 GitHub Pages 网页浏览。

### 文件命名
- Markdown：`reports/YYYY-MM-DD.md`
- HTML：`reports/YYYY-MM-DD.html`

### HTML 模板规范
参考 `reports/2026-03-13.html`，以下为固定规范：

**样式主题**
- 背景色 `#0f0f11`，卡片 `#1a1a1f`，强调色 `#6366f1`（靛蓝）
- 字体：`-apple-system, "PingFang SC", "Microsoft YaHei", sans-serif`
- 顶部导航含 Logo + `← 返回目录` 链接（指向 `/showcase/vibe-intel/`）

**内容结构（五节固定）**
1. `一、核心信号（Top 3）` — 多源印证用 `<span class="signal-badge">多源印证 ▲</span>` 标注
2. `二、新产品与技术动态` — 每个产品含：是什么 / 核心功能 / 目标用户 / 为何值得关注 / 链接
3. `三、开发者社区情绪` — 引用用 `<blockquote>` 样式
4. `四、资本与商业动向` — 有融资时用 `<table>` 展示（表头：公司 / 轮次金额 / 投资方 / 战略意义）
5. `五、分析师判断` — 本周趋势 / 今日最强信号 / 需持续观察

**页脚**
- 底部附 Markdown 原始文件的 GitHub 链接

### 更新首页目录
每新增一期 HTML 后，需同步更新 `index.html`：
- 在 `历史报告` 区域顶部插入新卡片（最新日期在前）
- 格式：`<a class="card" href="/showcase/vibe-intel/reports/YYYY-MM-DD.html">`

### 发布流程
```bash
cd ~/Documents/showcase
git add vibe-intel/reports/YYYY-MM-DD.html vibe-intel/index.html vibe-intel/README.md
git commit -m "feat(vibe-intel): add YYYY-MM-DD report HTML"
git push
```
GitHub Pages 会在约 1 分钟内自动部署。

### 访问地址
- 目录页：https://xiajngsi.github.io/showcase/vibe-intel/
- 单期报告：https://xiajngsi.github.io/showcase/vibe-intel/reports/YYYY-MM-DD.html
