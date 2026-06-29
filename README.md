<div align="center">

# 📖 Digital Life Lessons

### *Preserve Your Wisdom. Share Your Journey. Grow Together.*

[![Live Site](https://img.shields.io/badge/🌐_Live_Site-Visit_Now-4f46e5?style=for-the-badge)](https://your-live-url.com)
[![Client Repo](https://img.shields.io/badge/GitHub-Client_Repo-181717?style=for-the-badge&logo=github)](https://github.com/your-username/digital-life-lessons-client)
[![Server Repo](https://img.shields.io/badge/GitHub-Server_Repo-181717?style=for-the-badge&logo=github)](https://github.com/your-username/digital-life-lessons-server)

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Live URL](#-live-url)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [NPM Packages Used](#-npm-packages-used)
- [Pages & Routes](#-pages--routes)
- [MongoDB Collections](#-mongodb-collections)
- [Environment Variables](#-environment-variables)
- [Getting Started](#-getting-started)
- [Admin Credentials](#-admin-credentials)

---

## 🧠 About the Project

**Digital Life Lessons** is a full-stack web platform where users can create, store, and share meaningful life lessons, personal growth insights, and wisdom gathered over time. People often learn valuable lessons but forget them — this platform helps preserve personal wisdom, encourages mindful reflection, and allows users to grow by exploring lessons from a like-minded community.

Users can organize lessons, mark favorites, track learning progress, and browse public lessons shared by others. The platform features a **Free** and **Premium** tier powered by **Stripe**, and uses **Better Auth** for secure authentication.

---

## 🌐 Live URL

🔗 **[https://your-live-url.com](https://your-live-url.com)**

---

## ✨ Key Features

### 🔐 Authentication
- Email & Password registration with strong validation (uppercase, lowercase, min 6 chars)
- Google OAuth login via **Better Auth**
- JWT-based token verification on all protected routes
- Persistent login — no redirect on private route reload

### 📝 Lesson Management
- Create life lessons with **Title, Description, Category, Emotional Tone, Image, Visibility & Access Level**
- Categories: Personal Growth, Career, Relationships, Mindset, Mistakes Learned
- Emotional Tones: Motivational, Sad, Realization, Gratitude
- Visibility: Public / Private | Access Level: Free / Premium

### 💎 Free vs Premium System
- Free users can browse all public **Free** lessons
- Premium users unlock all **Premium** lessons
- Premium lessons shown as blurred/locked cards to Free users with upgrade prompt
- One-time ৳1500 lifetime upgrade via **Stripe Checkout**
- Webhook-based automatic role update after successful payment

### 🌍 Public Lesson Browsing
- Filter by category, emotional tone
- Sort by newest, most saved
- Search by title / keyword
- Paginated results

### 💬 Engagement & Interaction
- ❤️ Like / Unlike lessons (real-time, no refresh)
- 🔖 Save to Favorites (toggle)
- 💬 Comment on lessons
- 🚩 Report inappropriate lessons with reason dropdown
- 📤 Social sharing via `react-share`

### 📊 User Dashboard
- Overview: total lessons, favorites, recent activity, analytics chart
- Add / Edit / Delete own lessons
- Change visibility & access level
- My Favorites page with category/tone filters
- Profile management (name, photo)

### 🛠️ Admin Dashboard
- Platform-wide analytics: users, lessons, reports, growth graphs
- Manage users: promote to admin
- Manage lessons: feature on homepage, mark as reviewed, delete
- Handle reported/flagged lessons: delete or
This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
