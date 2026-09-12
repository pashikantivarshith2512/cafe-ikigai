# IKIGAI Café — Premium Full-Stack Café Platform & Management System
## Technical Stack & Architecture

- **Frontend:** Next.js (App Router), React 19, TypeScript, Tailwind CSS (Luxury Japanese Minimalist Design System), Framer Motion, Lucide Icons.
- **Backend:** Node.js, Express.js, TypeScript, REST APIs with Zod validation.
- **Database:** PostgreSQL with Prisma ORM.
- **Authentication & Security:** bcrypt password hashing, JWT sessions, Role-Based Access Control (`CUSTOMER`, `ADMIN`).
- **Features:** 
  - Interactive Database-Driven Menu (Coffee, Food, Desserts, Drinks)
  - Online Ordering & Shopping Cart Drawer
  - Delivery/Pickup options (Dine-in, Kerbside pickup, No-contact delivery)
  - Table Reservation Engine
  - Moderated Guest Reviews & Ratings
  - Instagram-style Photo Gallery
  - IKIGAI Loyalty Rewards Program
  - Newsletter Subscription Journal
  - AI Café Assistant Concierge
  - Comprehensive Admin Dashboard (Revenue, Orders pipeline, Reservations, Review moderation, Menu CRUD)
---
## Production Deployment Guide

1. **Database:** Deploy PostgreSQL on Neon, Supabase, or Railway. Copy connection string to production environment variables.
2. **Backend:** Deploy `backend` to Render or Railway with build command `npm run build` and start command `npm start`.
3. **Frontend:** Deploy `frontend` to Vercel with build command `npm run build`. Set `NEXT_PUBLIC_API_URL` pointing to backend domain.
