# MarketKit — Two-Sided Marketplace

MarketKit is a production-grade, two-sided marketplace starter kit. Built with **Next.js 16**, **Tailwind CSS v4**, and **Supabase**, it provides a complete foundation for developers to build, customize, and launch their own marketplace platforms—similar to Fiverr or Taskrabbit.

## 🚀 Vision

The goal of MarketKit is to provide a clean, modular, and scalable architecture that handles the "heavy lifting" of a marketplace (Auth, Stripe Connect, Admin Moderation, Real-time Chat) so you can focus on the unique value of your product.

---

## ✨ Features

### 👤 User Roles

- **Buyer**: Browse/search listings, book services via Stripe, real-time messaging, and review system.
- **Seller**: Listing management, availability settings, earnings dashboard, and automated payouts via Stripe Connect Express.
- **Admin**: Full moderation suite (approve/reject sellers and listings), platform analytics, and dispute resolution.

### 🛠 Core Functionality

- **Authentication**: Email & Google OAuth via Supabase Auth with Role-Based Access Control (RBAC).
- **Booking Flow**: End-to-end transaction flow (Pending → Confirmed → Completed).
- **Payments**: Integrated Stripe Connect for split payments and platform commissions.
- **Messaging**: Real-time chat system unlocked upon booking.
- **Reviews**: Verified purchase review system with star ratings.
- **Storage**: Image uploads for listings via Supabase Storage.
- **Notifications**: Automated email triggers via Resend.

---

## 🛠 Tech Stack

| Layer             | Technology                                                                       |
| :---------------- | :------------------------------------------------------------------------------- |
| **Frontend**      | [Next.js 16](https://nextjs.org/) (App Router), TypeScript                       |
| **Styling**       | [Tailwind CSS v4](https://tailwindcss.com/), [shadcn/ui](https://ui.shadcn.com/) |
| **Database/Auth** | [Supabase](https://supabase.com/) (PostgreSQL + RLS)                             |
| **Real-time**     | Supabase Realtime (Chat)                                                         |
| **Payments**      | [Stripe Connect Express](https://stripe.com/connect)                             |
| **Email**         | [Resend](https://resend.com/)                                                    |
| **Deployment**    | [Vercel](https://vercel.com/)                                                    |

---

## 🏁 Getting Started

### 1. Prerequisites

- Node.js 20+
- pnpm (recommended)
- Supabase Account
- Stripe Account
- Resend API Key

### 2. Installation

```bash
git clone https://github.com/mohamedafrash/market-kit.git
cd market-kit
pnpm install
```

### 3. Environment Setup

Create a `.env.local` file in the root directory:

```env
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key

# Stripe
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key

# Resend
RESEND_API_KEY=your_resend_key
```

### 4. Database Schema

Run the SQL migrations provided in the `/supabase` folder (coming soon) or use the Supabase dashboard to set up your tables:

- `profiles` (with `role` enum: buyer, seller, admin)
- `listings`
- `bookings`
- `messages`
- `reviews`

### 5. Start Developing

```bash
pnpm dev
```

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/FeatureName`)
3. Commit your Changes (`git commit -m 'Add some FeatureName'`)
4. Push to the Branch (`git push origin feature/FeatureName`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙌 Credits

- Built by [Afrash](https://github.com/mohamedafrash)
- UI components by [shadcn/ui](https://ui.shadcn.com/)
- Icons by [Lucide](https://lucide.dev/)
