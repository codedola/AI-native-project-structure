# 🚀 AI-Native E-Commerce Platform

[![Next.js](https://img.shields.io/badge/Next.js-14+-black?logo=next.js)](https://nextjs.org/)
[![NestJS](https://img.shields.io/badge/NestJS-10+-E0234E?logo=nestjs)](https://nestjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5+-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3+-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?logo=prisma)](https://www.prisma.io/)

An Enterprise-grade E-Commerce ecosystem built with an **AI-Native** philosophy. This project is designed to be co-authored by human developers and AI agents, utilizing a structured context management system.

---

## 🏗 System Architecture

The project follows a **Monorepo-style** architecture with clearly defined boundaries between frontend, backend, and admin dashboard.

- **Frontend (`apps/frontend`):** High-performance storefront using Next.js App Router and Server Components.
- **Backend (`apps/backend`):** Robust API layer powered by NestJS, Prisma ORM, and MySQL.
- **Admin Dashboard (`apps/dash`):** Internal management tool built with Next.js and Figma-driven UI components.
- **Infrastructure:** JWT + Redis for secure, real-time session management and Refresh Token Rotation.

> [!IMPORTANT]
> For deep technical details, check out [ARCHITECTURE.md](file:///.docs/ARCHITECTURE.md).

---

## 🤖 AI-Native Workflow (The "Secret Sauce")

This project is optimized for **Agentic Coding**. We use specialized "Skills" and a strict context management protocol to ensure the AI remains aligned with the system's architecture.

### Specialized Agentic Skills:
- **`/save`**: Automatically summarizes progress and updates [.docs/FEATURES_DONE.md](file:///.docs/FEATURES_DONE.md).
- **`/archive`**: Compresses memory, cleans logs, and updates core architecture documentation.

### The Developer-Agent Protocol:
1. **Context First**: Agents MUST read `ARCHITECTURE.md` and `FEATURES_DONE.md` at the start of every session.
2. **Design Fidelity**: All UI implementation must strictly follow [.docs/STYLEGUIDE.md](file:///.docs/STYLEGUIDE.md) and Figma/Stitch sources.
3. **No Yapping**: Communication is optimized for high-density information transfer (Token Optimization).

---

## 🛠 Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Core** | TypeScript (Strict Mode) |
| **Frontend** | Next.js 14+, React, Tailwind CSS, Tanstack Query |
| **Backend** | NestJS, Prisma, MySQL |
| **Caching/Security** | Redis (ioredis), JWT, Bcrypt |
| **Dev Tools** | AI Agent Skills, Custom MCP Servers |

---

## 📁 Project Structure

```text
.
├── .agent/              # 🤖 Agent definitions & specialized skills
│   ├── AGENTS.md        # Rules of engagement for AI Agents
│   └── skills/          # Executable automation scripts
├── .docs/               # 📄 Single Source of Truth documentation
│   ├── ARCHITECTURE.md  # System design & database schema
│   ├── STYLEGUIDE.md    # UI/UX & Tailwind standards
│   └── FEATURES_DONE.md # Real-time project progress log
├── apps/                # 🚀 Applications
│   ├── frontend/        # Storefront (Next.js)
│   ├── backend/         # API Gateway (NestJS)
│   └── dash/            # Admin Dashboard (Next.js)
└── README.md            # You are here
```

---

## 🚦 Getting Started

### Prerequisites
- Node.js 20+
- Docker (for MySQL & Redis)
- Your favorite AI Coding Assistant (optimized for this repo)

### Installation
```bash
# Clone the repository
git clone https://github.com/codedola/AI-native-project-structure.git

# Install dependencies (from root)
npm install
```

---

## 📜 Coding Standards

- **Zero `any`**: TypeScript strict mode is enforced.
- **Server Components**: Default to Server Components in Next.js; only use Client Components for interactivity.
- **Thin Controllers**: Business logic belongs in Services.
- **Security First**: Passwords are never stored in plain text; Refresh Token Rotation is mandatory.

---

*Built with ❤️ and 🤖 by the Antigravity Team.*
