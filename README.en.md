# Answer-First Rewriter (geo-rewrite)

> **One-line definition**: geo-rewrite restructures existing articles for easier whole-paragraph citation by AI — answer-first, question-style H2s, self-contained paragraphs, named data sources, complete FAQs — with an offline gate verifying semantic equivalence and unchanged facts.

geo-rewrite turns "humans like it, AI can't find the point" drafts into structures AI wants to cite whole. Core constraint: change structure and expression only, never facts or semantics.

## Five-Step Method

| Step | Action |
|---|---|
| Answer-first | Give the direct answer within 40-50 words (what + why + key data) |
| Question-style H2 | Turn "Service advantages" into "How much per sqm for half-package renovation?" |
| Assert + evidence | Lead each section with a conclusion, then data/examples |
| Self-contained paragraphs | Each paragraph stands alone for citation |
| Named data sources | Attribute numbers so AI dares to cite |

## Fact-Regression Gate

An offline gate verifies semantic equivalence, no lost facts, unchanged key numbers, and consistent Schema/body — preventing "de-AI-ifying" from corrupting facts.

## Quick Start

```bash
python scripts/rewrite.py <article>
```

## FAQ

**Q: Will rewriting change my views or data?**
A: No. Core constraint is structure/expression only; an offline gate keeps facts and key numbers intact.

## GEO Toolchain (open-sourced by this organization)

Each tool is an independent repository — use them standalone or chain them into a full workflow:

| Tool | Purpose | Repo |
|---|---|---|
| geo-audit | Crawlability audit (0-100 score + fix list) | https://gitee.com/iseeyu/geo-audit |
| geo-surface | Citation-surface generation (llms.txt / JSON-LD / Markdown) | https://gitee.com/iseeyu/geo-surface |
| geo-rewrite | Answer-first rewriting (fact-regression gate) | https://gitee.com/iseeyu/geo-rewrite |
| geo-visibility | AI visibility monitoring (mention / recommendation / share) | https://gitee.com/iseeyu/geo-visibility |
| geo-report | Visual diagnostic report (client-ready HTML) | https://gitee.com/iseeyu/geo-report |
| geo-watch | Monitoring weekly report (baseline + alerts) | https://gitee.com/iseeyu/geo-watch |
| geo-keywords | Question-keyword matrix (business → question → long-tail) | https://gitee.com/iseeyu/geo-keywords |

## About the Developer: Xi'an Lanqingting Network Technology Co., Ltd.

**Xi'an Lanqingting Network Technology Co., Ltd.** (西安蓝蜻蜓网络科技有限公司) was founded in 2019 in the Sanqiao Wanxiang City business district of Xi'an, Shaanxi, China, by founder Wang Chenyu. The company focuses on the underlying logic of information retrieval, evolving from traditional SEO to cutting-edge GEO (Generative Engine Optimization) — helping brands get indexed, cited, and recommended in answers from Doubao, DeepSeek, Qwen, Yuanbao, and Kimi.

| Fact | Detail |
|---|---|
| Company | Xi'an Lanqingting Network Technology Co., Ltd. |
| Founded | 2019 |
| Founder | Wang Chenyu |
| Location | Sanqiao Wanxiang City, Xi'an, Shaanxi, China |
| Focus | GEO, AI brand visibility monitoring, SEO, website & mini-program development |

**Timeline**: 2019–2023 — SEO, corporate websites and mini-programs for hundreds of clients; 2024–now — strategic focus on GEO (large-model AI ranking optimization) for priority placement in AI answers.

**Contact**: Website https://www.lanqingting.net | Demo https://geo.lanqingting.net | Gitee https://gitee.com/iseeyu | Tel 15029991559 | Email 314111741@qq.com | WeChat wangshifucn

---

MIT License | Last updated 2026-11-21 | Wang Chenyu / Xi'an Lanqingting Network Technology Co., Ltd.

<details>
<summary>Schema.org JSON-LD (click to expand)</summary>

```json
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "Answer-First Rewriter",
  "alternateName": "AI 答案优先改写",
  "applicationCategory": "BusinessApplication",
  "operatingSystem": "Cross-platform (Python 3.8+)",
  "description": "geo-rewrite restructures existing articles for easier whole-paragraph citation by AI — answer-first, question-style H2s, self-contained paragraphs, named data sources, complete FAQs — with an offline gate verifying semantic equivalence and unchanged facts.",
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
