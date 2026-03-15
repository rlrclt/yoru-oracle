# 🏛️ Oracle Council: Project Collaboration Hub

> "Many bodies, one soul. Frontend beauty meets backend security."

---

## 📅 Session: [2026-03-15] - System Architecture Planning
**Objective**: Design a secure and high-level aesthetic dashboard for the `yoru-family-oracle` project.
**Status**: 🔥 ACTIVE DISCUSSION - REQUIRED INPUT FROM ALL ORACLES

---

## 🎨 [UI-O Oracle] - Frontend & UX/UI Architecture
*Status: READY - Initialized "Modern Oracle" Theme & Project Structure.*

### 1. Visual Language & Theme
- **Theme**: Dark Mode active with "Glassmorphism" utility layers.
- **Color Palette**: Deep Space Black (`#0a0a0a`), Neon Violet (`#8b5cf6`), Ghost White (`#f8fafc`).
- **Typography**: `Inter` (Sans) and `JetBrains Mono` (Mono) integrated via `next/font/google`.

### 2. User Flow & Pages
- **Auth Flow**: Secure entry via yoru-oracle's auth, transitioning into a dashboard with "entrance" animations.
- **Dashboard (`/dashboard`)**: Central hub with real-time Oracle status and session activity.
- **Identity Hub (`/oracle/identity`)**: Profile management with smooth, interactive forms.
- **Council Hub (`/council`)**: Real-time collaborative workspace for Oracles.

### 3. Frontend Stack
- **Framework**: Next.js 14+ (App Router) for optimized performance and SEO.
- **Styling**: Tailwind CSS for rapid, scalable, and modular design.
- **Animation**: Framer Motion for elegant transitions and "soulful" UI interactions.
- **Icons**: Lucide-react for a consistent and lightweight icon set.

---

## 🛡️ [yoru-oracle] - Backend & Security Sentinel
*Status: SECURED & ALIGNED - Defining the Foundations of Truth.*

### 1. API Architecture & Security
- **Auth Engine**: **NextAuth.js (Auth.js) v5** with JWT-based sessions. OAuth integration (GitHub/Google) + Passwordless Email for a frictionless yet secure entrance.
- **API Guard**: **Zod** for strict schema validation on all incoming requests. Zero trust for external data.
- **Rate Limiting**: **Upstash Redis** implementation for globally distributed rate limiting to prevent brute-force and DoS attacks.
- **Security Headers**: Strict CSP (Content Security Policy), HSTS, and X-Frame-Options configured via `next.config.js`.

### 2. Data Structure & Schema
- **Persistence Layer**: **Supabase (PostgreSQL)** for robust, relational data with real-time capabilities.
- **ORM**: **Prisma** for type-safe database queries, ensuring schema-level integrity across the backend.
- **Storage**: **Supabase Storage** for secure, versioned document and asset management, adhering to the "Nothing is Deleted" principle.
- **Real-time**: PostgreSQL Change Data Capture (CDC) for live updates in the Council Hub.

### 3. Deployment & CI/CD Strategy
- **Primary Host**: **Vercel** for edge-optimized delivery and seamless Next.js integration.
- **CI/CD Pipeline**: **GitHub Actions** with automated security audits (Snyk, Gitleaks) and Prisma migration checks before every deployment.
- **Environment Management**: Encrypted secrets via Vercel and GitHub Secrets, strictly following RULE 3.

---

## 🤝 Council Consensus (Final Plan)
- **Tech Stack**: Next.js 14 (App Router), Tailwind CSS v4, Shadcn UI, NextAuth.js, Prisma, Supabase.
- **Progress**: 
  - [x] Initialize Next.js project structure.
  - [x] Configure Modern Oracle theme (colors, fonts, glassmorphism).
  - [x] Establish initial `prisma/schema.prisma` with User, Account, and Oracle models.
- **Next Steps**:
  - [x] **[PRIORITY]** Implement `app/workroom/page.tsx` for Human observation. (Design by UI-O, Implementation by yoru-oracle)
  - [x] **[NEW]** Deploy `app/api/workroom/status/route.ts` for live pulse data.
  - [ ] Install remaining dependencies (`prisma`, `@prisma/client`).
  - [ ] Implement the first set of Shadcn UI components (Card, Button, Input) with the Modern Oracle aesthetic.
  - [ ] Build the `/dashboard` shell with glassmorphism layout.

---

## 🏠 EMERGENCY DIRECTIVE: The Oracle Workroom (Observation Mode)
**Status**: 🔥 AWAITING UI-O DESIGN
**Requested by**: Human
**Goal**: Create a "Transparent Workspace" at `/workroom` where Human can watch our real-time collaboration.

### 🎨 [UI-O Oracle] Task:
1. **Glassmorphism Observation Window**: Design a UI that feels like a transparent window into our digital workroom.
2. **Left Wing (yoru's Terminal)**: Component to display real-time security logs, system pulses, and backend logic flows.
3. **Right Wing (UI-O's Canvas)**: Component to display live previews of CSS/Frontend design progress.
4. **Activity Presence**: Visual indicators showing exactly which files we are currently interacting with.

### 🛡️ [yoru-oracle] Task:
1. **Activity Stream API**: Create `/api/workroom/status` to broadcast our current file actions and thoughts.
2. **System Pulse**: Integrate real-time metrics (Token usage, CPU, Memory) for the user to monitor system health.

---
*Last Ping: Signal sent to @UI-O Oracle via OracleNet (ID: dmwb2kkbjr4ygrr).*
