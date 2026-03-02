# 🛠 MarketKit Feature Roadmap & Checklist

This document tracks the progress of the MarketKit marketplace. Check off items as they are completed.

---

## 🏗 Phase 1: Foundation & Infrastructure
- [ ] **Project Setup**
  - [x] Next.js 16 + Tailwind v4 + shadcn/ui Initialization
  - [x] Project Documentation (README, LICENSE)
  - [ ] GitHub Repository & CI/CD (Vercel)
- [ ] **Database & Auth (Supabase)**
  - [ ] Initialize Supabase Project
  - [ ] Setup Database Schema (Profiles, Listings, Bookings, Reviews)
  - [ ] Configure Row Level Security (RLS) Policies
  - [ ] Email & Google OAuth Configuration
- [ ] **Shared Layouts & UI Primitives**
  - [ ] Main Navigation (Responsive)
  - [ ] Footer
  - [ ] Core shadcn components (Button, Input, Card, Dialog, Toast)

---

## 🔑 Phase 2: Authentication & User Profiles
- [ ] **Onboarding Flow**
  - [ ] Role Selection (Buyer vs. Seller) on Signup
  - [ ] User Profile Page (View/Edit)
- [ ] **Seller Specifics**
  - [ ] Seller Onboarding (Stripe Connect Express integration)
  - [ ] Seller Profile Verification state

---

## 🛍 Phase 3: Listings & Search (The Marketplace Core)
- [ ] **Listing Management**
  - [ ] Create Listing Form (multi-step with Image Uploads)
  - [ ] Listing Approval Workflow (Pending -> Approved/Rejected)
  - [ ] Manage Listings Dashboard for Sellers
- [ ] **Discovery**
  - [ ] Homepage with Featured Categories
  - [ ] Search Page with Filters (Category, Price, Rating)
  - [ ] Listing Detail Page (Description, Seller Info, Reviews)

---

## 💳 Phase 4: Booking & Payments
- [ ] **Checkout Flow**
  - [ ] Booking Calendar/Quantity selection
  - [ ] Stripe Checkout Session Integration
  - [ ] Payment Webhook handling (captured vs. failed)
- [ ] **Transaction Management**
  - [ ] Buyer Dashboard (My Bookings)
  - [ ] Seller Dashboard (Manage Requests/Orders)
  - [ ] Booking Status Updates (Confirmed -> Completed)
  - [ ] Commission logic (Platform fee)

---

## 💬 Phase 5: Interaction & Reviews
- [ ] **Real-time Messaging**
  - [ ] Unlock Chat after Booking
  - [ ] Message Notification Badges
  - [ ] Real-time UI updates via Supabase
- [ ] **Feedback System**
  - [ ] Post-completion Review Form
  - [ ] Star Rating Calculation on Profile/Listings

---

## 🛡 Phase 6: Admin Moderation & Analytics
- [ ] **Admin Dashboard**
  - [ ] Seller Application Queue
  - [ ] Listing Moderation Queue
  - [ ] Platform Statistics (Total GMV, Users, Active Listings)
  - [ ] Dispute/Refund Manual Trigger

---

## 📧 Phase 7: Notifications & Polish
- [ ] **Email System (Resend)**
  - [ ] Booking Confirmation Email
  - [ ] Payout Released Email
  - [ ] Notification on New Message
- [ ] **Visual Polish**
  - [ ] Loading Skeletons for all data-heavy pages
  - [ ] Error Boundary states
  - [ ] Empty States for dashboards (e.g., "No bookings yet")

---

## 🚢 Phase 8: Launch Prep
- [ ] **Testing**
  - [ ] E2E Test of Booking Flow
  - [ ] RLS Security Audit
- [ ] **Final Deployment**
  - [ ] Production Environment Variables
  - [ ] Domain Setup
