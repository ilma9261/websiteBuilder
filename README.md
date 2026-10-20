# 🚀 GenWeb.ai — AI Website Builder

Describe a website in plain English and get a **complete, responsive, multi-page website** in seconds. Preview it live, edit the code, chat with the AI to make changes, and publish it with one click.


---

## ✨ Features

- 🤖 **AI website generation** — type a prompt, get a full HTML/CSS/JS site (Home, About, Services, Contact)
- 💬 **Chat-based editing** — ask the AI for changes ("make the navbar dark", "add a pricing section")
- 👀 **Live preview** — see the website instantly in the browser
- 🧑‍💻 **Built-in code editor** — view and read the generated code (Monaco Editor, same as VS Code)
- 🌐 **One-click deploy** — each website gets its own shareable link (`/site/your-site`)
- 🔐 **Google login** — secure sign-in with Firebase + JWT cookies
- 💳 **Credits & payments** — free credits for every user, paid plans through Stripe
- 📱 **Responsive output** — generated sites work on mobile, tablet and desktop

---

## 🛠️ Tech Stack

| Part | Technology |
|------|------------|
| Frontend | React 19, Vite, Tailwind CSS 4, Redux Toolkit, React Router, Framer Motion |
| Backend | Node.js, Express 5 |
| Database | MongoDB + Mongoose |
| Auth | Firebase Google Sign-In, JWT (HTTP-only cookies) |
| AI | OpenRouter API (DeepSeek model) |
| Payments | Stripe Checkout + Webhooks |
| Editor | Monaco Editor |

---

## ⚙️ How It Works

1. User signs in with Google
2. User writes a prompt describing the website
3. Backend sends the prompt to the AI and gets back a full HTML page
4. The website is saved in MongoDB and shown in a live preview
5. User can keep chatting with the AI to update it
6. User clicks **Deploy** and gets a public link

**Credits:** every new user gets 100 free credits. Generating a website costs 50 credits and each update costs 25.

| Plan | Price | Credits |
|------|-------|---------|
| Free | ₹0 | 100 |
| Pro | ₹499 | 500 |
| Enterprise | ₹1499 | 1000 |

---

## 📁 Project Structure

```
websiteBuilder/
├── client/                 # React frontend
│   └── src/
│       ├── pages/          # Home, Dashboard, Generate, Editor, Pricing, LiveSite
│       ├── components/     # Login modal
│       ├── redux/          # Global user state
│       └── hooks/          # Fetch the logged-in user
└── server/                 # Express backend
    ├── controllers/        # Auth, website, billing, Stripe webhook
    ├── models/             # User and Website schemas
    ├── routes/             # API routes
    ├── middlewares/        # JWT auth check
    └── config/             # Database, AI, Stripe, plans
```

---

## 🧠 What I Learned

- Building a full-stack **MERN** app from scratch
- Writing prompts that make an AI return **structured JSON** reliably
- Handling **authentication** with Firebase and JWT cookies
- Integrating **Stripe payments and webhooks** to manage a credit system
- Managing global state with **Redux Toolkit**

---


