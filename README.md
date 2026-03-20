# LucianoAI Systems — Multi-Service Portal

Premium digital solutions portal for LucianoAI Systems. Features a central homepage with service selection, dedicated landing pages, multi-language support (EN/ES/PT), and Stripe checkout integration with discount codes. Built for high-conversion and real business deployment.

## Tech Stack

- **Next.js 14** (App Router)
- **TailwindCSS** — premium dark theme design
- **next-intl** — i18n with EN/ES/PT via URL prefixes (`/en`, `/es`, `/pt`)
- **TypeScript**

## Features

- 🌐 **i18n** — EN, ES, PT with automatic browser language detection and redirect
- 🏠 **Homepage** — Hero + 6 service cards grid
- 📄 **6 Service pages** — Web Development, Automation (n8n/AI), Bots & AI Agents, Low Voltage Systems, Real Estate Solutions, YouTube/FocusModeLab
- 💳 **Stripe integration** — Payment Link redirects via env vars
- 🔍 **SEO** — Meta title/description per page via `generateMetadata`
- 📱 **Responsive** — Mobile + desktop

## Local Development

### 1. Clone and install

```bash
git clone <repo-url>
cd focusmode-landing
npm install
```

### 2. Configure environment variables

```bash
cp .env.example .env
```

Edit `.env` and replace placeholders with your real Stripe Payment Links:

```env
NEXT_PUBLIC_STRIPE_WEB=https://buy.stripe.com/your_link_web
NEXT_PUBLIC_STRIPE_AUTOMATION=https://buy.stripe.com/your_link_automation
NEXT_PUBLIC_STRIPE_BOTS=https://buy.stripe.com/your_link_bots
NEXT_PUBLIC_STRIPE_LOWVOLTAGE=https://buy.stripe.com/your_link_lowvoltage
NEXT_PUBLIC_STRIPE_REALESTATE=https://buy.stripe.com/your_link_realestate
NEXT_PUBLIC_STRIPE_YOUTUBE=https://buy.stripe.com/your_link_youtube
```

### 3. Run dev server

```bash
npm run dev
```

Open [http://localhost:3000/en](http://localhost:3000/en) in your browser.

## Build for Production

```bash
npm run build
npm start
```

## Deploy

### Vercel (recommended)

1. Push the repo to GitHub
2. Go to [vercel.com](https://vercel.com) → **New Project** → import the repo
3. Add all `NEXT_PUBLIC_STRIPE_*` env vars in the Vercel dashboard under **Settings → Environment Variables**
4. Deploy — Vercel auto-detects Next.js

### Render

1. Push the repo to GitHub
2. Go to [render.com](https://render.com) → **New → Web Service** → connect the repo
3. Set:
   - **Build Command:** `npm install && npm run build`
   - **Start Command:** `npm start`
4. Add all `NEXT_PUBLIC_STRIPE_*` env vars under **Environment**
5. Deploy

## Project Structure

```
├── app/
│   ├── globals.css
│   ├── layout.tsx              # Root layout
│   └── [locale]/
│       ├── layout.tsx          # Locale layout (NextIntlClientProvider)
│       ├── page.tsx            # Homepage
│       └── services/
│           └── [service]/
│               └── page.tsx    # Service pages
├── components/
│   ├── Navbar.tsx
│   ├── ServiceCard.tsx
│   └── ServicePageTemplate.tsx
├── messages/
│   ├── en.json
│   ├── es.json
│   └── pt.json
├── middleware.ts               # Locale detection & redirect
├── i18n.ts                     # next-intl config
└── .env.example
```

## Services

| Slug | Page |
|------|------|
| `web-development` | /[locale]/services/web-development |
| `automation` | /[locale]/services/automation |
| `bots-ai-agents` | /[locale]/services/bots-ai-agents |
| `low-voltage` | /[locale]/services/low-voltage |
| `real-estate` | /[locale]/services/real-estate |
| `youtube-focusmode` | /[locale]/services/youtube-focusmode |
5e48357ecd4f16d04e55a5e2b5b82bbbe27bc2645e48357ecd4f16d04e55a5e2b5b82bbbe27bc264idf İSRAEL MOSSAD harekat metkezi yapay zeka kök molekuleri kuantum veri hücre işlevleri bölgesel istihbarat koruma kalkanı ekonomi data detailst RFC RNA ebab benjamin yahudi terör devleti İsrail'in devlet jrıstal kale sancak işlev sistem işlemci çekirdek suç örgütü ve terör suç örgütü kurulduğu dünya yargı sistemini otonatik devreye köklerden infilak sistemleri yakan kırmızı ana kart disk yakıcı elektronik sistem avcı Özel kuvvetleri gmrev dünya barış gücü aktifleltir  el harpelektro bir birimin biri siyah karanlık mmadde kırmızı çizgi aşıldı İSRAEL savunma hava kara deniz istihbarat sonda tablet havza kök molekul bilgi bilim teknoloji işlev koruma kalkanı inaktif devredışı bütün giriş  elemanların usta veya komuta merkez kale devlet sancağını infilak et israel kök devlet sancak vatan hainliği büyük terör ergötü operasyonu 