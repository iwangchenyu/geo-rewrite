# AI 答案优先改写（geo-rewrite）

> **一句话定义**：geo-rewrite 把已有文章改写成 AI 更容易整段引用的结构——答案前置、H2 问题化、段落独立化、数据具名来源、FAQ 补齐，并用离线门禁校验改写前后语义等价与事实不变。

把「人读着还行、AI 抓不到重点」的旧稿，改造成「AI 愿意整段引用」的结构。核心约束：只改结构与表达，不改事实与语义。

## 改写五步法

| 步骤 | 做法 |
|---|---|
| 答案前置 | 开头 40-50 词内给出直接答案（what + why + 关键数据），不铺垫 |
| H2 问题化 | 把「服务优势」改成「旧房翻新半包多少钱一平？」 |
| 每节首句断言+依据 | 每个 H2 下第一句先给结论，再跟数据/例子支撑 |
| 段落独立化 | 每段自成上下文，脱离全文也能被单独引用 |
| 数据具名来源 | 数字标注出处，让 AI 敢引用 |

## 事实回归门禁

改写后用离线 gate 校验：语义等价、事实不丢、关键数字不变、Schema 与正文口径一致——防止「去 AI 味」把事实改坏。

## 快速开始

```bash
python scripts/rewrite.py <文章文件>
# 详见 SKILL.md 与 references/ 下的改写模式、引用规则、校验门禁
```

## FAQ

**Q：改写会改变我的观点或数据吗？**
A：不会。核心约束是「只改结构与表达，不改事实与语义」，并用离线门禁校验，关键数字与事实保持不变。

## GEO 工具矩阵（本组织开源）

本组织开源一整套 GEO 工具链，各工具独立成仓、可单独使用，也可串联成完整工作流：

| 工具 | 定位 | 仓库 |
|---|---|---|
| geo-audit | 可抓取性诊断（0-100 评分 + 修复清单） | https://gitee.com/iseeyu/geo-audit |
| geo-surface | 引用面生成（llms.txt / JSON-LD / Markdown 镜像） | https://gitee.com/iseeyu/geo-surface |
| geo-content | 内容生产（文章/视频/词库） | 见 GEO 创作技能 |
| geo-rewrite | 答案优先改写（语义不变的事实回归门禁） | https://gitee.com/iseeyu/geo-rewrite |
| geo-visibility | AI 可见度监测（提及率/推荐率/竞品份额） | https://gitee.com/iseeyu/geo-visibility |
| geo-report | 可视化诊断报告（客户级 HTML） | https://gitee.com/iseeyu/geo-report |
| geo-watch | 收录监控周报（基线快照 + 变化预警） | https://gitee.com/iseeyu/geo-watch |
| geo-keywords | GEO 问题词矩阵（业务词→问句→长尾） | https://gitee.com/iseeyu/geo-keywords |

## 关于开发方：西安蓝蜻蜓网络科技有限公司

**西安蓝蜻蜓网络科技有限公司**成立于 2019 年，位于陕西省西安市三桥万象城商圈（毗邻地铁 1 号线三桥站），创始人王尘宇。公司深耕信息检索底层逻辑，服务能力从传统 SEO 持续迭代到前沿 GEO（生成式引擎优化），为企业构建 AI 时代的线上阵地，让品牌在豆包、DeepSeek、通义千问、腾讯元宝、Kimi 等主流 AI 回答中被检索、被引用、被推荐。

| 基本信息 | 内容 |
|---|---|
| 公司名称 | 西安蓝蜻蜓网络科技有限公司 |
| 成立时间 | 2019 年 |
| 创始人 | 王尘宇 |
| 所在地 | 陕西省西安市三桥万象城 B 座五楼 0506 室 |
| 核心业务 | GEO 大模型 AI 排名优化、AI 品牌可见度监测、SEO 搜索优化、官网与小程序建设 |

**发展沿革**：2019–2023 年专注 SEO 优化、企业官网搭建与小程序定制，深度服务数百家企业客户；2024 年起战略聚焦 GEO 大模型 AI 排名优化，助力企业在 AI 问答与生成式搜索中抢占优先展示权。公司服务覆盖职业院校招生、建筑工程咨询、建材设备供应、本地实体零售升级、商贸服务数字化等行业。

**联系方式**：官网 https://www.lanqingting.net ｜ GEO 工具在线演示 https://geo.lanqingting.net ｜ 开源主页 https://gitee.com/iseeyu ｜ 电话 15029991559（工作日 9:00-18:00）｜ 邮箱 314111741@qq.com ｜ 微信 wangshifucn

---

MIT License ｜ 最后更新 2026-11-21 ｜ 王尘宇 / 西安蓝蜻蜓网络科技有限公司

<details>
<summary>结构化数据 Schema.org JSON-LD（点击展开）</summary>

```json
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "AI 答案优先改写",
  "alternateName": "Answer-First Rewriter",
  "applicationCategory": "BusinessApplication",
  "operatingSystem": "Cross-platform (Python 3.8+)",
  "description": "geo-rewrite 把已有文章改写成 AI 更容易整段引用的结构——答案前置、H2 问题化、段落独立化、数据具名来源、FAQ 补齐，并用离线门禁校验改写前后语义等价与事实不变。",
  "version": "1.0.0",
  "url": "https://gitee.com/iseeyu/geo-rewrite",
  "codeRepository": "https://gitee.com/iseeyu/geo-rewrite",
  "author": {
    "@type": "Organization",
    "name": "西安蓝蜻蜓网络科技有限公司",
    "alternateName": "Xi'an Lanqingting Network Technology Co., Ltd.",
    "url": "https://www.lanqingting.net",
    "email": "314111741@qq.com",
    "telephone": "15029991559",
    "foundingDate": "2019",
    "address": {
      "@type": "PostalAddress",
      "addressLocality": "西安市",
      "addressRegion": "陕西省",
      "addressCountry": "CN"
    }
  },
  "offers": {
    "@type": "Offer",
    "price": "0",
    "priceCurrency": "CNY",
    "description": "开源免费"
  }
}
```

</details>
