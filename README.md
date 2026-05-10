# Traveloop

Traveloop is an AI-powered travel planning platform built with Next.js.  
It helps users design trips end-to-end: itinerary building, city/activity planning, budgeting, checklists, notes, sharing, and community discovery.

---

## 🌐 Live Website

🚀 The project is successfully deployed and live at:  
👉 https://aetherius-ten.vercel.app/

---


## ✨ Project Highlights

- Secure authentication with role-based access (`user`, `admin`)
- Multi-trip dashboard and trip lifecycle management
- Multi-stop itinerary builder with reorder support
- Activity planning and destination discovery
- Budget and carbon-related assistant APIs
- AI assistant for trip ideas, cost reduction, and planning help
- Notes and checklist tools for execution readiness
- Community sharing flows
- Admin analytics dashboard (usage, trends, engagement, user management)

---

## 🛠 Tech Stack

- Frontend: Next.js 14 (App Router), React 18, Tailwind CSS, Framer Motion
- State/Data: Zustand, TanStack Query
- Backend/API: Next.js Route Handlers
- Database: MongoDB with Mongoose models
- Cache/Rate Limit: Upstash Redis (optional in local dev)
- AI Provider: Hugging Face Inference Router
- Charts: Recharts

---

## 🏗 Architecture Notes

- App structure:
  - `app/(auth)` → login/signup
  - `app/(dashboard)` → main product
  - `app/api/v1/*` → backend APIs
- JWT-based authentication
- AI APIs in `app/api/v1/ai/*`
- Admin dashboard: `/admin`

---

## ⚙️ Setup

```bash
npm install
cp .env.local.example .env
npm run dev
