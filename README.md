# Awesome-Enterprise-Content-Discovery

# Awesome-Enterprise-Content-Discovery

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Federated Search, AI-Powered Knowledge Discovery, Permission-Aware Retrieval & RAG**
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Content Discovery**. These tools help employees find documents, answer questions, and discover knowledge across disconnected systems—SharePoint, Confluence, Google Drive, Slack, databases, and more—without manually searching each source.

**Examples** include Microsoft Delve, Glean, Coveo, Sinequa, Lucidworks Fusion, Elastic Enterprise Search, Guru, Algolia, BA Insight, and Swiftype (the category leaders).

**Open-source emphasis**: The open-source enterprise search ecosystem is **mature and production-proven**. **Onyx** (formerly Danswer) is the closest open-source alternative to Glean, offering self-hosted deployment, 40+ connectors, permission-aware retrieval, and generated answers with citations . **Turing CE** provides a self-hosted alternative to Algolia and Coveo with hybrid BM25+vector ranking, RAG chat, AI agents, and MCP tools . **Fess** delivers full-text enterprise search on OpenSearch with crawlers for web, file, database, and cloud sources . **SWIRL** federates search across 100+ apps without moving data—no vector database, no ETL, no second copy to govern .

## 📖 Table of Contents

- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)
- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#how-to-contribute)
- [⚠️ Disclaimer](#-disclaimer)

## ☁️ SaaS/Hosted Platforms

> **📊 Market Context**: The global enterprise search and content discovery market is estimated at **~$8B in 2026**, growing toward **~$20B by 2032**. The sector is **moderately fragmented** — **Glean** leads the AI-native enterprise search category with a **$7.2B valuation** , while **Coveo**, **Sinequa**, and **Lucidworks** dominate the traditional enterprise search tier, and **Microsoft Delve** leverages Microsoft 365 distribution. **Pricing varies dramatically**: Glean has **no public pricing** and requires enterprise sales engagement, Elastic Enterprise Search offers a **free Basic tier** with **30-day trial** for paid features, and **Algolia** starts with a **free tier (10,000 search requests/month)** . No single vendor holds a winner-take-all position; enterprises typically run multi-vendor stacks.

| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |
|----------|-------------|------------------------|------------------|--------------|
| **[Microsoft Delve](https://www.microsoft.com/en-us/microsoft-365/delve)** | **Microsoft's content discovery tool.** Surfaces relevant documents and colleagues based on Microsoft Graph signals. | **Bundled with Microsoft 365** (E3/E5) subscriptions. No standalone purchase. | **Included with Microsoft 365** at no additional cost. Requires active M365 subscription. | **~$281B revenue (Microsoft FY2025)** |
| **[Glean](https://www.glean.com/)** | **AI-native enterprise search and work assistant.** 100+ connectors, Enterprise Knowledge Graph, permission-aware retrieval, and AI agents. **$7.2B valuation** . | **No public pricing** — quote required. Enterprise sales engagement only. | **No free tier**. **Demo** required. | **$7.2B valuation, $600M+ raised**  |
| **[Coveo](https://www.coveo.com/)** | **AI-powered relevance platform.** Relevance Generative AI for synthesized answers with citations, Case Assist AI for support deflection. | **Custom enterprise pricing** — quote required. | **None** — enterprise demo required. | **Public (CVO), ~$200M+ revenue est.** |
| **[Sinequa](https://www.sinequa.com/)** | **Enterprise search and analytics platform.** Natural language processing, machine learning, and 200+ connectors. | **Custom enterprise pricing** — quote required. | **None** — enterprise demo required. | **Private (~$100M+ revenue est.)** |
| **[Lucidworks Fusion](https://lucidworks.com/)** | **AI-powered search platform.** Connectors, relevance tuning, and RAG capabilities. | **Custom enterprise pricing** — quote required. | **Free trial** available on request. | **Private (~$100M+ raised)** |
| **[Elastic Enterprise Search](https://www.elastic.co/enterprise-search)** | **Elastic's enterprise search suite.** App Search, Workplace Search, and Site Search. | **Free Basic tier** available. **Platinum**: **$95/month** (starting). **Enterprise**: **$109/month** . | **Free Basic tier**: Available for self-managed. **30-day trial** for paid features. | **Public (ESTC), ~$1.5B revenue** |
| **[Guru](https://www.getguru.com/)** | **AI-powered knowledge management.** Verified answers surfaced in Slack, browser, and other tools. | **Custom pricing** — quote required. Entry plans typically **$15–$25/user/month**. | **Free trial** available. **No perpetual free tier**. | **Private (~$100M+ raised)** |
| **[Algolia](https://www.algolia.com/)** | **Search and discovery API.** Sub-50ms response times, NeuralSearch, and Recommend. | **Free tier** with limits. **Grow**: **$1/month** (10,000 requests). **Grow Plus**: **$0.50/1K requests** after 100K . | **Free tier**: **10,000 search requests/month**, 1 million records, 100,000 AI credits. **14-day free trial** for paid plans . | **Private (~$2.25B valuation est.)** |
| **[BA Insight](https://www.bainsight.com/)** | **Enterprise search and AI platform.** Connectors for Microsoft 365, Salesforce, and more. | **Custom enterprise pricing** — quote required. | **None** — enterprise demo required. | **Private** |
| **[Swiftype](https://swiftype.com/)** | **Site search and enterprise search (acquired by Elastic).** Now part of Elastic Enterprise Search. | **N/A** — merged into Elastic Enterprise Search. | **N/A** — merged into Elastic. | **Part of Elastic** |

## 🔓 Open-Source GitHub Projects

| Repo | Description | Stars |
|------|-------------|-------|
| **[Onyx (formerly Danswer)](https://github.com/onyx-dot-app/onyx)** — **The closest open-source alternative to Glean.** Self-hosted internal search across **40+ connectors** including Salesforce, GitHub, Google Drive, Confluence, Slack, and Notion . **MIT licensed**, free community edition with **no seat minimum** . **Permission-aware retrieval** respects source permissions. **Generated answers with citations** using your choice of LLM. **Companies running in about 30 minutes**. Used by **Netflix, Ramp, and Thales Group** . | [![Stars](https://img.shields.io/github/stars/onyx-dot-app/onyx?style=social&color=white)](https://github.com/onyx-dot-app/onyx/stargazers) | ~15,000 |
| **[Turing CE (Viglet)](https://github.com/openviglet/turing-ce)** — **Self-hosted Apache-2.0 alternative to Algolia and Coveo.** **Faceted semantic search**, **hybrid BM25+vector ranking** fused with **Reciprocal Rank Fusion**, **RAG chat with inline source citations**, **AI agents with MCP tools**, and a React admin console. **Multi-engine**: one API over **Apache Solr, Elasticsearch, or embedded Lucene**. **Indexes Adobe AEM, WordPress, databases, and files** via Viglet Dumont connectors. **Runs fully offline** for regulated/air-gapped deployments . | [![Stars](https://img.shields.io/github/stars/openviglet/turing-ce?style=social&color=white)](https://github.com/openviglet/turing-ce/stargazers) | ~500 |
| **[Fess](https://github.com/codelibs/fess)** — **Open-source, self-hosted enterprise search server built on OpenSearch.** **Crawls web, file, DB, and cloud sources** including Confluence, Jira, Box, Dropbox, G Suite, Office 365, S3, Salesforce, SharePoint, and Slack . **Full-text search with faceting**, sorting, and suggestions. **Role- and permission-based filtering**. **SSO with LDAP, OpenID Connect, SAML, SPNEGO, and Microsoft Entra ID**. **20+ languages**. **Apache-2.0** . | [![Stars](https://img.shields.io/github/stars/codelibs/fess?style=social&color=white)](https://github.com/codelibs/fess/stargazers) | ~1,000 |
| **[SWIRL Community](https://github.com/swirlai/swirl-search)** — **Federated AI search and RAG without moving your data.** **Apache-2.0**, free to self-host. **Queries your sources live** with the user's own permissions—**no vector database, no ETL, no second copy to govern** . **100+ connectors** including Microsoft 365, Google, AWS Kendra, Confluence, Jira, SharePoint, Slack, Salesforce, ServiceNow, and more . **Galaxy UI**, real-time RAG with citations, and cosine vector re-ranking . **One Docker command, about 2 minutes** . | [![Stars](https://img.shields.io/github/stars/swirlai/swirl-search?style=social&color=white)](https://github.com/swirlai/swirl-search/stargazers) | ~1,500 |
| **[Datafari](https://github.com/francelabs/datafari)** — **Open-source intelligent enterprise search engine (Apache-2.0).** **Datafari 7.0** adds an **AI assistant for conversing with documents**, **RAG mode** for answers grounded only in internal data, and an **agentic mode** for AI reasoning . **Keyword, semantic, and hybrid search modes** . **Administer connectors via Apache ManifoldCF** . **AI at indexing** for content analysis and enrichment . **Email alerts** when new or modified documents match a query . | [![Stars](https://img.shields.io/github/stars/francelabs/datafari?style=social&color=white)](https://github.com/francelabs/datafari/stargazers) | ~500 |
| **[OpenBeam](https://github.com/kuluruvineeth/openbeam)** — **Open-source Glean for SaaS and the physical world.** **87 connectors** including Slack, GitHub, Notion, Linear, Salesforce, Jira, Gmail, plus **IoT (Samsara, Verkada, AWS IoT)** and **industrial protocols (MQTT, OPC-UA, BACnet)** . **Hybrid semantic + keyword search** with sub-200ms p99 latency. **AI agents with 100+ composable tools**. **MCP server** for Claude Code, Cursor, and Codex. **Permission-aware** and **self-hostable** via Docker Compose. **AGPL** licensed . | [![Stars](https://img.shields.io/github/stars/kuluruvineeth/openbeam?style=social&color=white)](https://github.com/kuluruvineeth/openbeam/stargazers) | ~500 |
| **[Omo](https://github.com/omo-ai/omo)** — **Open-source, AI-native enterprise search.** **LLM and vector store agnostic**—configure GPT, Llama 3, Claude, or Gemini via environment variable . **Connectors**: Google Drive, Notion, Confluence, Airtable, OneDrive, Slack . **Declarative pipelines** defined in YAML. **Hybrid search** returns ranked links plus generative AI answer. **Source citations** for every answer. **Slack client** and multi-tenancy support. **Apache-2.0** . | [![Stars](https://img.shields.io/github/stars/omo-ai/omo?style=social&color=white)](https://github.com/omo-ai/omo/stargazers) | ~500 |
| **[Redrob Recall](https://github.com/redrob-labs/redrob-recall)** — **Local-first desktop app for searching your files and asking grounded questions.** **Everything stays on device**—files, extracted text, embeddings, and the complete search index . **Indexes selected folders** without Docker or a separate database. **Reads PDF, DOCX, TXT, Markdown, RST, CSV, JSON, HTML, XML, and log files** . **Combines multilingual semantic retrieval with keyword matching**. **Produces answers with numbered citations back to local files** . **Tauri 2 + React 19 + SQLite FTS5 + Qdrant Edge** . | [![Stars](https://img.shields.io/github/stars/redrob-labs/redrob-recall?style=social&color=white)](https://github.com/redrob-labs/redrob-recall/stargazers) | ~200 |

**Additional open-source options worth exploring:**

| Repo | Description |
|------|-------------|
| **[Hister](https://github.com/asciimoo/hister)** — Private full-content search index under your control. Stores complete content of chosen webpages and files on your own server. Browser extension, local folder monitoring, browsing history import, and website crawling. Full-text search with field filters, wildcards, date ranges. Optional semantic search. **AGPLv3**, single binary, SQLite/PostgreSQL, Docker, MCP server . |
| **[lazylens](https://pypi.org/project/lazylens/)** — Fast terminal lens over work knowledge. Local SQLite/FTS index over Confluence, Jira, and local folders. Cross-source relationship navigation between Confluence pages and Jira issues. Textual TUI . |
| **[DocFetcher](https://docfetcher.sourceforge.io/)** — Cross-platform desktop search application. Indexes folders and searches file contents across PDF, Office, OpenOffice, RTF, CHM, Visio, SVG, and Outlook PST files. Boolean, wildcard, phrase, and fuzzy search. Full Unicode support . |
| **[Elastic Enterprise Search](https://github.com/elastic/enterprise-search)** — Elastic's enterprise search suite including App Search, Workplace Search, and Site Search. Free Basic tier available for self-managed deployments . |

## 🤝 How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## ⚠️ Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Enterprise content discovery platforms handle sensitive organizational knowledge and user data; ensure proper access controls, permission mapping, and compliance with data protection regulations.
- **Open-source reality**: The open-source ecosystem for enterprise content discovery is **mature and production-proven**. **Onyx** is the closest open-source alternative to Glean with 40+ connectors and permission-aware retrieval, used by Netflix and Ramp . **Turing CE** provides a self-hosted Apache-2.0 alternative to Algolia and Coveo with hybrid ranking and RAG chat . **Fess** delivers full-text enterprise search on OpenSearch with crawlers for Confluence, Jira, SharePoint, and more . **SWIRL** federates search across 100+ apps without moving data—no vector database, no ETL . However, **commercial platforms** (Glean, Coveo, Sinequa) provide **managed infrastructure, curated relevance engineering, and dedicated support** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong engineering capacity seeking data sovereignty and cost control.
- **Deployment caveat**: Open-source enterprise search replaces the license line with an **operations line**—you own upgrades, scaling, connector maintenance, and identity mapping for every source you add . **Onyx runs in about 30 minutes** to start, but production deployments require ongoing ownership .

---

**Made for IT administrators, knowledge managers, DevEx teams, and enterprise architects.**
Let's make enterprise content discovery more open, transparent, and accessible.
