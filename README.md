# IKIGAI Café — Premium Full-Stack Café Platform & Management System

> **Brand:** IKIGAI Café  
> **Philosophy:** IKIGAI represents the Japanese philosophy of finding purpose, balance, and joy in everyday moments.  
> **Category:** Premium Coffee Shop / Luxury Café & Kitchen (Kondapur, Hyderabad)  
> **Rating:** 4.4 ⭐ (671+ Verified Reviews)  
> **Price Range:** ₹400–1400 per person  
> **Address:** Ground Floor of M.R PRIME Building (LEEWAY), Kondapur, Laxmi Cyber City, Whitefields, Gachibowli, Hyderabad, Telangana 500084  
> **Phone:** 098490 00120 | **Website:** cafeikigai.com

---

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



## PostgreSQL Database Setup & Seeding

1. Configure your PostgreSQL connection string in `backend/.env`:
   ```env
   "
   ```

2. Run Prisma schema generation and push migrations:
   ```bash
   cd backend
   npx prisma generate
   npx prisma db push
   ```

3. Seed database with authentic IKIGAI Café data (Admin user, Sample customer, Categories, Menu items, Reviews, Gallery):
   ```bash
   npm run prisma:seed
   ```

---


---

## Running the Application Locally

### Backend Server:
```bash
cd backend
npm run dev
# Starts REST API on http://localhost:5000
```

### Frontend Website:
```bash
cd frontend
npm run dev
# Starts Next.js Web App on http://localhost:3000
```

---

## Production Deployment Guide

1. **Database:** Deploy PostgreSQL on Neon, Supabase, or Railway. Copy connection string to production environment variables.
2. **Backend:** Deploy `backend` to Render or Railway with build command `npm run build` and start command `npm start`.
3. **Frontend:** Deploy `frontend` to Vercel with build command `npm run build`. Set `NEXT_PUBLIC_API_URL` pointing to backend domain.
