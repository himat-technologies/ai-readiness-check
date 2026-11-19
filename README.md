<div align="center">

# ✨ AI Readiness Check

### Make your website easier for AI to find, understand, and recommend.

An AI-search readiness auditor by **Himat Technologies**. Check any public website for crawlability, technical SEO, structured data, content signals, performance, and AI crawler access.

<a href="https://himat.tech/free-tools/ai-readiness-check"><strong>🚀 Try the live demo</strong></a>

<br />

![Next.js](https://img.shields.io/badge/Next.js-15-111827?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-Ready-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge)

</div>

---

## 🌈 What it does

Enter a website URL and get a practical report showing how well that site is prepared for AI-powered search experiences. The results include an overall score, category breakdowns, detailed checks, crawler access, and prioritized recommendations.

| 🔎 Audit area | 📋 What is checked |
|:---|:---|
| **Crawlability** | Robots directives and AI crawler access |
| **Sitemap health** | Sitemap discovery and availability |
| **Technical SEO** | Essential page-level SEO signals |
| **Content quality** | Content signals that help systems understand a page |
| **AI discoverability** | Signals used by AI search platforms |
| **Performance** | Performance-related indicators |

## 💡 Features

- **Live website analysis** through `POST /api/analyze`
- **Weighted AI Readiness Score** from 0–100 across six categories
- **Clear audit results** with pass, warning, and fail checks
- **Actionable recommendations** with suggested fixes
- **Platform compatibility** for ChatGPT, Google AI Overviews, Perplexity, Gemini, Claude, and Bing Copilot
- **AI crawler detection** including GPTBot, ClaudeBot, and PerplexityBot
- **Structured data inspection** for JSON-LD, Microdata, and RDFa
- **Report exports** in JSON and PDF, plus a copyable summary
- **Scan history** saved in browser `localStorage`
- **Responsive, colorful interface** with Himat Technologies contact links

## 🧰 Built with

| Frontend | Analysis & reporting |
|:---|:---|
| Next.js 15 · React 19 · TypeScript | Cheerio · Axios · `robots-parser` |
| Tailwind CSS · shadcn-style UI primitives | `fast-xml-parser` · `pdf-lib` |
| React Hook Form · Zod | Recharts · Sonner · Lucide React |

## ⚡ Quick start

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Available scripts

```bash
npm run dev     # Start the development server
npm run build   # Create a production build
npm start       # Run the production server
npm run lint    # Run ESLint
```

### Environment

Environment variables are optional for local scans. If needed, copy `.env.example` to `.env.local`:

```bash
cp .env.example .env.local
```

## 🔌 API

### `POST /api/analyze`

Request:

```json
{
  "url": "https://example.com"
}
```

A successful response includes `success`, `score`, `categories`, `checks`, `recommendations`, `crawlers`, `schemas`, `platforms`, and the full `report` object.

## 📊 Score guide

| Score | Rating |
|:---:|:---|
| 🟢 **90–100** | Excellent |
| 🔵 **75–89** | Good |
| 🟠 **50–74** | Needs improvement |
| 🔴 **0–49** | Poor |

| Category | Weight |
|:---|:---:|
| Crawlability | 20% |
| Sitemap health | 15% |
| Technical SEO | 20% |
| Content quality | 15% |
| AI discoverability | 15% |
| Performance signals | 15% |

## 🗂️ Project structure

```text
app/                  App Router pages and API
  api/analyze/        Website analysis endpoint
components/
  charts/             Score gauge and category chart
  dashboard/          Score dashboard and loading skeletons
  forms/              URL analysis form
  layout/             Hero, FAQ, CTA, and footer
  reports/            Audit, recommendations, exports, and history
  ui/                 Shared UI primitives
hooks/                Analysis and scan-history hooks
lib/
  analyzers/          Fetch, robots, sitemap, SEO, content, schema, performance
  scoring/            Weighted scoring engine
  site.ts             Himat brand and contact configuration
  export.ts           JSON summary and PDF generation
types/                Shared TypeScript types
```

## 🤝 About Himat Technologies

<div align="center">

| 🌐 Website | ✉️ Email | 📞 Contact | 🚀 Live demo |
|:---:|:---:|:---:|:---:|
| [himat.co.in](https://himat.co.in) | [info@himat.co.in](mailto:info@himat.co.in) | [94452 34023](tel:+919445234023) | [AI Readiness Check](https://himat.tech/free-tools/ai-readiness-check) |

### Connect with us

[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/people/Himat-technologies/61593829197445/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/himat-technologies-14b1051b4)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/himat_technologies?stkn=djdmcGxweWtwYWI0)

</div>

## 📄 License

See [LICENSE](./LICENSE).

<div align="center">

**Built with care by [Himat Technologies](https://himat.co.in) · [Try the demo](https://himat.tech/free-tools/ai-readiness-check)**

</div>
