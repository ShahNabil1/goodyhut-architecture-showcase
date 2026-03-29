# 🛒 GoodyHut.bd - Enterprise B2B Import, CRM & E-Commerce Platform

> 🔒 **Confidentiality Notice:** The source code for this project is private to protect proprietary business logic. This repository serves as an architectural showcase demonstrating the advanced system design, backend infrastructure, and automated workflows I engineered for the platform.

## 🚀 System Overview
GoodyHut.bd is a highly scalable, production-grade e-commerce platform designed to handle complex B2B import logistics, real-time marketing automation, and dynamic front-end rendering. As the Lead Full-Stack Architect, I utilized AI-assisted UI generation (Lovable) powered by a heavily customized, self-hosted-capable **Supabase** backend, **Vercel Edge Functions**, and advanced Server-Side Tracking protocols.

## 🛠️ Core Tech Stack & Infrastructure
<p align="left">
  <img src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="React" />
  <img src="https://img.shields.io/badge/typescript-%23007acc.svg?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/supabase-%233ECF8E.svg?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=Cloudinary&logoColor=white" alt="Cloudinary" />
</p>

---

## 🧠 Core Engineering & Architecture Highlights

### 1. Advanced Authentication & Granular RBAC
* **OTP & OAuth:** Integrated **BulkSMSBD API** with a verified Sender ID for seamless BD phone login, OTP verification, and password resets. Integrated Google OAuth for quick access.
* **Strict RLS & Dynamic RBAC:** Implemented Row Level Security (RLS) for data isolation. Built a highly dynamic Role-Based Access Control (RBAC) panel where Super Admins can promote users to Admins/Moderators and explicitly restrict or grant access to specific pages within the admin dashboard.

### 2. Logistics, Fraud Detection & Order Automation
* **Fraud Prevention:** Integrated **BD Courier API** to instantly check customer phone numbers against a national courier fraud database during order processing.
* **One-Click Fulfillment:** Built a "Send to Steadfast" integration. With one click in the admin panel, complete order details are pushed to the Steadfast API, instantly returning the Consignment ID and Tracking ID.
* **Dynamic Shipping Calculator:** Engineered an auto-calculation logic for shipping charges based on specific product categories and estimated weights, ensuring 100% transparent checkout.
* **Payment Gateway:** Securely integrated **SSLCommerz** for digital transactions.

### 3. Smart CRM, Wallet & Abandoned Cart Recovery
* **Comprehensive CRM Dashboard:** Admins can view complete customer profiles (LTV, order history, saved cart items, last login, registration date).
* **Customer Wallet & Custom Coupons:** Built a digital wallet system for seamless refund processing (usable in future checkouts). Admins can generate custom coupons (Flat/Percentage, Min. Purchase, Max Use, Expiry) and assign them directly to specific users.
* **Abandoned Cart Recovery:** The database auto-saves checkout drops (items, qty, total, shipping). CRM operators can directly call, WhatsApp, or offer targeted discounts to recover these sales.

### 4. Automated Notifications & Marketing Automation
* **Real-Time Alerts:** Integrated **Resend API** (Emails) and **BulkSMSBD API** (SMS). Customers receive automated, dynamic template-based updates for every order status change. Admins get real-time alerts for new orders.
* **Personalized Bulk SMS Campaigns:** Admins can send personalized promotional SMS (using `{name}` attributes) directly from the CRM.
* **Smart Filtering & Cron Jobs:** The SMS engine automatically filters out duplicate numbers, inactive users, and frequent returners. A custom **Cron Job** ensures delivery reliability by retrying failed SMS every 1 hour for up to 24 hours.

### 5. Advanced SEO, Middleware OG & Server-Side Tracking
* **Flawless Meta CAPI & GA4:** Implemented strict Server-Side Tracking for events (Page view, registration, add to cart, checkout, search). Engineered **Event Deduplication** using unique Event IDs to prevent double-counting between Meta Pixel and Conversions API.
* **Dynamic Feeds & Sitemaps:** Automatically generated and real-time updating XML feeds for Facebook Catalog and dynamic `sitemap.xml` for Google Search Console, alongside optimized `robots.txt`.
* **Vercel Middleware for Dynamic SEO:** Utilized Vercel Middleware to dynamically intercept share requests. When a product is shared on social media, the middleware generates accurate Open Graph (OG) Images, Meta Titles, and Meta Descriptions on the fly, keeping the root URL clean (`goodyhut.bd`).
* **AI-Powered SEO Generation:** Integrated an AI API in the admin panel to automatically read product names, images, specs, and descriptions to generate the best Meta Titles, Meta Descriptions, and 15-20 bilingual (English/Bangla) search tags in one click.

### 6. AI Vector Search & Dynamic Frontend Management
* **Smart Image Search:** Built an advanced vector search feature allowing users to upload an image and instantly find visually similar products in the database.
* **Zero-Code Frontend Updates:** The admin panel allows instant creation of Deals and Campaign pages, application of special discounts, and dynamic editing of all legal pages (About Us, Refund Policy, TOS) and footer details without touching the codebase.

---

## 🤝 Let's Connect
I build highly complex, scalable systems that solve real business bottlenecks. If you are looking for an architect who understands enterprise logic, automated marketing, and secure backend operations, let's talk.

* 🌐 **Portfolio:** [shahnabil.com](https://shahnabil.com)
* ✉️ **Email:** hello@shahnabil.com
