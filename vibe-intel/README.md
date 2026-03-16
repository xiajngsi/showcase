# 🌐 Vibe Coding & AI 情报日报
> 每日追踪 vibe coding、agent engineering 市场动态  
> 网页版：https://xiajngsi.github.io/showcase/vibe-intel/

## 📅 历史报告
- [2026-03-16](reports/2026-03-16.md) · [HTML](reports/2026-03-16.html)
- [2026-03-15](reports/2026-03-15.md) · [HTML](reports/2026-03-15.html)
- [2026-03-14](reports/2026-03-14.md) · [HTML](reports/2026-03-14.html)
- [2026-03-13](reports/2026-03-13.md) · [HTML](reports/2026-03-13.html)

---

## 📋 HTML 同步规则（每日必做）

> **核心原则：每一期 Markdown 简报，必须同步生成对应 HTML 文件，并更新首页目录。**

### 1. 文件命名
| 类型 | 路径 |
|------|------|
| Markdown 原稿 | `reports/YYYY-MM-DD.md` |
| HTML 网页版 | `reports/YYYY-MM-DD.html` |
| 首页目录 | `index.html` |

### 2. HTML 生成规范

参考 `reports/2026-03-13.html`，以下为固定规范：

**样式主题（禁止修改）**
- 背景 `#0f0f11`，卡片 `#1a1a1f`，强调色 `#6366f1`
- 字体：`-apple-system, "PingFang SC", "Microsoft YaHei", sans-serif`
- 顶部导航：Logo + `← 返回目录`（链接指向 `/showcase/vibe-intel/`）

**内容五节结构**
1. `一、核心信号（Top 3）` — 多源印证标注用 `<span class="signal-badge">多源印证 ▲</span>`
2. `二、新产品与技术动态` — 每条目：是什么 / 核心功能 / 目标用户 / 为何值得关注 / 🔗 链接
3. `三、开发者社区情绪` — 引用语录用 `<blockquote>` 标签
4. `四、资本与商业动向` — 有融资时用 `<table>` 展示（表头：公司 / 轮次金额 / 投资方 / 战略意义）
5. `五、分析师判断` — 本周趋势 / 今日最强信号 / 需持续观察

**页眉/页脚**
- 顶部：日期徽章 + 标题 + 信源数量（meta 行）
- 底部：Markdown 原始文件的 GitHub 链接

### 3. 首页目录更新（index.html）

每期新 HTML 完成后，在 `index.html` 的报告列表**顶部**插入新卡片（最新在前）：

```html
<a class="card" href="/showcase/vibe-intel/reports/YYYY-MM-DD.html">
  <div class="card-date">📅 YYYY-MM-DD</div>
  <div class="card-title">Vibe Coding & Agent Engineering 市场情报简报</div>
  <div class="card-arrow">→</div>
</a>
```

### 4. 发布流程

```bash
cd ~/Documents/showcase
git add vibe-intel/reports/YYYY-MM-DD.html vibe-intel/index.html vibe-intel/README.md
git commit -m "feat(vibe-intel): add YYYY-MM-DD report HTML"
git push
```

GitHub Pages 约 **1 分钟**内自动部署生效。

### 5. 访问地址
- 目录页：https://xiajngsi.github.io/showcase/vibe-intel/
- 单期报告：https://xiajngsi.github.io/showcase/vibe-intel/reports/YYYY-MM-DD.html
