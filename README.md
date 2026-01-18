# 🧠 CrewAI Knowledge Base Builder
**Powered by CrewAI + OpenAI**

> **Transform Confluence chaos into structured knowledge. Connect your space, let 5 AI agents analyze your docs, and get a clean information architecture with canonical articles—automatically.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-15.1-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![CrewAI](https://img.shields.io/badge/CrewAI-Multi_Agent-purple.svg)](https://crewai.io/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

CrewAI Knowledge Base Builder is an intelligent documentation platform that uses a **5-agent CrewAI workflow** to:

1. **Collect Content** — Fetch all pages, markdown, and metadata from your Confluence space
2. **Classify & Cluster** — Group related pages by topic and content similarity
3. **Architect Structure** — Design a clean information architecture with logical hierarchy
4. **Write Articles** — Draft comprehensive canonical articles from clustered pages
5. **Edit & Refine** — Polish content for clarity, consistency, and quality

All in a beautiful, modern interface with real-time progress tracking.

---

## 🎯 Core Features

### 🤖 **Multi-Agent AI Workflow**
- **5 Specialized Agents** — Collector, Classifier, OutlineArchitect, Writer, Editor
- **Real OpenAI Integration** — gpt-4.1-mini for intelligent content analysis
- **Visual Progress Tracking** — Watch agents work in real-time with animated stepper
- **Typewriter Effect** — AI responses animate character-by-character

### 📊 **Knowledge Base Tools**
- **Confluence Browser** — Navigate and select spaces directly in-app
- **IA Tree Visualization** — Interactive tree view of proposed structure
- **Content Clustering** — See which source pages map to each canonical article
- **Export to Confluence** — Push structured KB back to Confluence (coming soon)

### 🎨 **Modern UI/UX**
- **Single-Page Architecture** — Smooth state-driven transitions, no page reloads
- **Dark/Light Mode** — Beautiful themes with system preference support
- **Mobile-First Design** — Responsive with 44px+ touch targets
- **Framer Motion Animations** — Delightful micro-interactions throughout

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🔐 **Optional Auth** | Sign in to save projects, or use anonymously |
| 📁 **Project Management** | Create, organize, and track KB projects |
| 🕐 **Run History** | View past runs with search and filters |
| 💬 **Quick Start Widget** | Try the AI without navigating away from homepage |
| 👥 **Collaboration Ready** | Real-time presence indicators |
| 🌓 **Theme Toggle** | Light/dark mode with persistence |
| 📱 **Bottom Navigation** | Mobile-optimized navigation |
| ⚡ **Agent Progress** | Live visual tracking of agent execution |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 15.1** | React 19.2 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **Framer Motion** | Smooth animations |
| **Lucide Icons** | Modern icon set |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **CrewAI** | Multi-agent AI orchestration |
| **OpenAI gpt-4.1-mini** | Intelligent analysis |
| **Pydantic v2** | Data validation |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL persistence |
| **Upstash Redis** | Job queue & caching |

### **External APIs** 🔌
| API | Purpose |
|-----|---------|
| **Confluence Cloud** | Documentation source |
| **OpenAI** | AI-powered analysis |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│       Confluence Space Key + Root Page (optional)           │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                  CREWAI WORKFLOW                            │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │  Collector   │  │  Classifier  │  │   Outline    │      │
│  │    Agent     │──│    Agent     │──│   Architect  │      │
│  │ (Fetch docs) │  │  (Cluster)   │  │  (Design IA) │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
│                                             │               │
│                    ┌────────────────────────┴────┐          │
│                    ▼                             ▼          │
│             ┌──────────────┐              ┌──────────────┐  │
│             │    Writer    │              │    Editor    │  │
│             │    Agent     │─────────────│    Agent     │  │
│             │ (Draft docs) │              │  (Refine)    │  │
│             └──────────────┘              └──────────────┘  │
└─────────────────────────────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • Information Architecture Tree                            │
│  • Content Clusters with Topics                             │
│  • Canonical Articles per Cluster                           │
│  • Page Mapping (old → new)                                 │
└─────────────────────────────────────────────────────────────┘
```

---

## 📖 User Guide

### Getting Started

1. **Open the App** — Visit the homepage or click "Try It Now"
2. **Browse Confluence** — Use the Confluence Browser to select your space
3. **Choose Root Page** — Optionally select a root page to narrow scope
4. **Run Analysis** — Watch the 5 agents process your documentation
5. **Explore Results** — View IA tree, clusters, and canonical articles

### Understanding the Agents

| Agent | Role | Output |
|-------|------|--------|
| **Collector** | Fetches all pages and content | Page data, metadata |
| **Classifier** | Groups related pages | Topic clusters |
| **OutlineArchitect** | Designs hierarchy | IA tree structure |
| **Writer** | Drafts canonical articles | Article content |
| **Editor** | Polishes and refines | Final articles |

### Pro Tips

- **Start small** — Test with spaces of ≤50 pages first
- **Use root pages** — Narrow scope for faster, focused results
- **Check clusters** — Review which pages map to each canonical article
- **Iterate** — Run multiple times with different root pages

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Easy on the eyes (default)
- 🖥️ **System** — Follows OS preference

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Analysis Time | ~15-30 seconds |
| Frontend Bundle | Optimized |
| Lighthouse Score | 90+ |
| Mobile Ready | ✅ Yes |

---

## 🛡️ Security

- ✅ Confluence credentials never exposed to frontend
- ✅ All API operations proxied server-side
- ✅ Environment variables for all secrets
- ✅ Input sanitization and validation
- ✅ Rate limiting support (Redis-based)

---

## 🔧 Recent Enhancements

### Jaw-Dropping Features ✨
1. **Typewriter Effect** — AI messages animate character-by-character
2. **Agent Progress Tracker** — Visual stepper showing real-time execution
3. **Interactive Agent Cards** — Hover effects with personality details
4. **OpenAI Integration** — Real AI conversations with gpt-4.1-mini
5. **Confluence Browser** — Modal UI to browse and select spaces
6. **Quick Start Widget** — Floating widget for instant interaction

### Advanced Features 🚀
7. **Optional Authentication** — Sign in to save, or use anonymously
8. **Project Management** — Create, organize, track KB projects
9. **IA Tree Visualization** — Interactive documentation structure
10. **Export to Confluence** — Push results back (UI ready)
11. **Run History** — Searchable past runs with filters
12. **Real-time Collaboration** — Presence indicators and cursors

### Mobile Optimizations 📱
- 44px+ touch targets on all interactive elements
- Bottom navigation with 4 key routes
- Responsive layouts that stack on mobile
- Touch-friendly modals and controls

---

## 👨‍💻 Creator

**Derril Filemon**

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — CrewAI multi-agent workflows, OpenAI gpt-4.1
- ⚛️ **Modern React** — Next.js 15.1, React 19.2, App Router, Server Components
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic
- 🎨 **UI/UX Design** — Responsive design, animations, accessibility
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, monitoring
- 🔗 **API Integration** — Confluence Cloud REST API

---

## 🙏 Acknowledgments

- **[CrewAI](https://crewai.io/)** — Multi-agent AI orchestration
- **[OpenAI](https://openai.com/)** — gpt-4.1-mini API
- **[Confluence](https://www.atlassian.com/software/confluence)** — Documentation platform
- **[Supabase](https://supabase.com/)** — Database & auth
- **[Upstash](https://upstash.com/)** — Redis caching
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful components
- **[Framer Motion](https://www.framer.com/motion/)** — Animations

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
