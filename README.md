# 🚀 Hireek — Modern SaaS Recruitment Platform

**Hireek** is a full-featured SaaS recruitment platform connecting companies and job seekers with ease. Built using the latest technologies, Hireek delivers a seamless, fast, and secure hiring experience.

Whether you're an employer looking to post jobs and manage applicants, or a job seeker searching for the next big opportunity, Hireek has you covered.

---

## 🌟 Features at a Glance

### ✅ General
- ⚡ Built with **Next.js 15 App Router**
- 🎨 Styled using **TailwindCSS** & **shadcn/ui**
- 🌙 Dark/Light mode support
- 🔐 Secure authentication via **Google** & **GitHub OAuth** (Auth.js)
- 💾 Serverless database with **Prisma + Neon Postgres**
- 📦 Managed with **pnpm**

### 🏢 Company Dashboard
- Guided onboarding flow for company setup
- Create, edit, and manage job postings
- Review & manage candidate applications
- View job post details and expiration workflows
- Mark favorite candidates and job seekers

### 🙋 Job Seeker Dashboard
- Profile creation with resume uploads
- Browse and apply to jobs
- Track application history
- Favorite job posts
- Receive notifications and updates

### ⚙️ Power Features
- 📬 **Inngest** for background job expiration and workflows
- 🛡️ **Arcjet** for runtime security and bot protection
- 💳 **Stripe** integration for payments
- 📤 File uploads via **UploadThings**
- 🧩 Fully modular CRUD functionality
- 🧱 Beautiful skeleton loaders for improved UX
- 🚀 Deployed on **Vercel** with edge performance

---

## 📁 Tech Stack

| Area              | Tech                                      |
|-------------------|-------------------------------------------|
| Frontend Framework | [Next.js 15](https://nextjs.org/)         |
| Styling           | [Tailwind CSS](https://tailwindcss.com/), [shadcn/ui](https://ui.shadcn.dev/) |
| Authentication    | [Auth.js](https://authjs.dev/)            |
| ORM & Database    | [Prisma](https://prisma.io/) + [Neon](https://neon.tech/) |
| File Uploads      | [UploadThings](https://uploadthing.com/)  |
| Security          | [Arcjet](https://arcjet.com/)             |
| Background Jobs   | [Inngest](https://inngest.com/)           |
| Payments          | [Stripe](https://stripe.com/)             |
| Deployment        | [Vercel](https://vercel.com/)             |
| Package Manager   | [pnpm](https://pnpm.io/)                  |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/ayoubhayda/hireek-platform.git
cd hireek-platform
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Configure Environment Variables

Create a .env.local file in the root of the project and fill it with your configuration. You can use the provided .env.example as a reference.

```bash
cp .env.example .env.local
```

Update the following variables with your own credentials:

```bash
# This is your Auth.js secret. You can generate a new one using `npx auth generate-secret`.
AUTH_SECRET="" # Added by `npx auth`. Read more: https://cli.authjs.dev


# Auth with Google Credentials
AUTH_GOOGLE_ID=""
AUTH_GOOGLE_SECRET=""


# Auth with GitHub Credentials
AUTH_GITHUB_ID=""
AUTH_GITHUB_SECRET=""

# This is your Neon database connection string. You can find it in your Neon dashboard.
DATABASE_URL=""

# This is your Uploadthing token. You can find it in your Uploadthing dashboard.
UPLOADTHING_TOKEN=""

# This is your Arcjet key. You can find it in your Arcjet dashboard.
ARCJET_KEY=""

# This is secret key for Stripe. You can find it in your Stripe dashboard.
SECRET_STRIPE_KEY=""

# This is base URL for your app.
NEXT_PUBLIC_BASE_URL=

# This is secret key for Stripe webhook. You can find it in your Stripe dashboard.
STRIPE_WEBHOOK_SECRET=""

# This is your Resend API key. You can find it in your Resend dashboard.
RESEND_API_KEY=""
```

### 4. Run Prisma Migrations

```bash
pnpm dlx prisma db push
```

### 5. Start the Development Server

```bash
pnpm run dev
```

## 📦 Scripts

| Command                 | Description               |
|-------------------------|---------------------------|
| pnpm run dev            | Start development server  |
| pnpm run build          | Build for production      |
| pnpm run start          | Start production server   |
| pnpm run lint           | Lint the codebase         |
| pnpm dlx prisma studio  | Open Prisma Studio        |

## 🧪 Testing

Unit and integration tests coming soon. Testing tools planned:
- Jest
- Playwright for E2E
- Testing Library

## 🌐 Deployment

Hireek is optimized for seamless deployment to [Vercel](https://vercel.com/). Just connect your GitHub repo, set up the environment variables, and you're live.

Alternatively, you can deploy to any other Node.js-compatible platform that supports environment variables and PostgreSQL.

## 🙌 Built With Love, Backed by Power

- Next.js – App Router, SSR, RSC
- Prisma – Powerful database access layer
- Neon – Scalable serverless Postgres
- Inngest – Zero-cron background tasks
- Arcjet – Enterprise-grade security
- UploadThings – Seamless file uploads
- Tailwind CSS – Modern, utility-first styling
- Shadcn/UI – Accessible component library
- Vercel – Lightning-fast global deployment

## ⭐️ Star the Repo

If you like Hireek, consider starring the repo to support the project and spread the word!