# TheTop36.com – Hybrid Raffle + Vault Engine

## 📌 Overview

**TheTop36.com** is a web platform that sells curated public-domain PDF bundles for $7, each purchase granting users a raffle entry to win branded prizes. The system is designed to drive revenue and user engagement over a 45-day cycle using a hybrid model of digital product delivery and micro-lottery mechanics.

---

## 🚀 Features

- 🎯 Landing page with product bundles and branding
- 💳 Stripe integration for secure $7 purchases
- 🎟️ Raffle entry generation after successful purchase
- 🧠 Random winner selection after 100 entries
- 📩 Email notifications to winners and participants (MailerLite or SMTP)
- 🛠️ Admin dashboard to track tickets, winners, and email logs

---

## 🧑‍💻 Tech Stack

- **Frontend:** React / Next.js + Tailwind CSS
- **Backend:** Node.js + Express.js
- **Payments:** Stripe API
- **Email:** MailerLite or Nodemailer (SMTP fallback)
- **Deployment:** Vercel (Frontend) + Replit or Railway (Backend if separated)

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/thetop36-raffle-engine.git
cd thetop36-raffle-engine
2. Install Dependencies
bash
Copy
Edit
npm install
3. Environment Variables
Create a .env file in the root directory with the following:

ini
Copy
Edit
STRIPE_SECRET_KEY=sk_test_51RWbO7SB4VL9D52XD0YQUbb4KdtjadSQpI41b9fgTkDGSJV6A0Dcrbu2J79xupgfOikQS58eFoBloiOjvpdp9vHz00AaKt7WrM
STRIPE_WEBHOOK_SECRET=your_webhook_secret
EMAIL_API_KEY=your_mailerlite_or_smtp_key
EMAIL_FROM=noreply@thetop36.com
4. Run the App
bash
Copy
Edit
npm run dev
🧪 Testing
Test Stripe payment flow using test card: 4242 4242 4242 4242

Confirm raffle ID generation and email notifications

Check admin dashboard for ticket and winner info
