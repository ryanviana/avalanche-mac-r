# Avalanche MAC Redirect

![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?logo=tailwindcss&logoColor=white)

A link redirect and click-tracking service for the MAC (Avalanche blockchain) project. Routes short reference URLs to their target destinations while tracking unique clicks per IP for pay-per-click analytics.

## How It Works

1. A user visits `/<reference>` (e.g., `/my-link`)
2. The app looks up the reference in the backend API and retrieves the target URL
3. Unique IP clicks are recorded for analytics
4. The user is redirected to the destination

## Tech Stack

- **Next.js 14** (Pages Router + App Router)
- **MongoDB / Mongoose** for link-reference storage
- **Backend API** hosted on Vercel (`backend-mac.vercel.app`)
- **Tailwind CSS** for styling

## Getting Started

```bash
npm install
```

Create a `.env` file with your MongoDB connection string and any required API keys.

Run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.
