# ⚡ ZenBot Pro v2.0

[![Next.js 15](https://img.shields.io/badge/Next.js-15.0_App_Router-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma)](https://prisma.io)
[![Binance API](https://img.shields.io/badge/Binance-Live_&_Testnet-F0B90B?style=for-the-badge&logo=binance)](https://binance.com)
[![Telegram](https://img.shields.io/badge/Telegram-Instant_Alerts-26A5E4?style=for-the-badge&logo=telegram)](https://telegram.org)
[![Stripe](https://img.shields.io/badge/Stripe-Checkout_&_Webhooks-635BFF?style=for-the-badge&logo=stripe)](https://stripe.com)
[![Bilingual i18n](https://img.shields.io/badge/i18n-English_%26_Português-10B981?style=for-the-badge)](https://kiptecnologia.github.io/zenbot-pro/)
[![By Kip Tecnologia](https://img.shields.io/badge/By-Kip_Tecnologia-059669?style=for-the-badge)](https://github.com/KipTecnologia)
[![Live Demo](https://img.shields.io/badge/Live-Demo_Ready-emerald?style=for-the-badge&logo=googlechrome)](https://kiptecnologia.github.io/zenbot-pro/)

> **English**: Turnkey **Algorithmic Cryptocurrency Trading, Visual Backtesting & Automation Micro-SaaS Boilerplate**. Built with **Next.js 15 App Router**, **TypeScript**, **Prisma ORM**, **Binance Testnet & Live Connector**, **Telegram Alert Webhooks**, and **Stripe Subscriptions**.  
> **Português**: Plataforma comercial pronta de **Trading Algorítmico de Criptomoedas, Backtesting Visual e Automação de Sinais**. Construído com **Next.js 15**, **Prisma ORM**, **Conexão Binance Testnet/Live**, **Alertas no Telegram** e **Stripe**. Engineered by **[Kip Tecnologia](https://github.com/KipTecnologia)**.

---

## ⚡ Live Interactive Demo (Bilingual EN / PT)

Experience the live visual trading dashboard with real-time simulated orderbook and strategy backtesting:  
👉 **[https://kiptecnologia.github.io/zenbot-pro/](https://kiptecnologia.github.io/zenbot-pro/)**

- **📊 Candlestick & Volume Charts**: Real-time rendering with indicators (RSI, MACD, Bollinger Bands) and buy/sell signals.
- **⚡ Binance Testnet Connector**: Seamless integration for paper trading and zero-risk strategy execution.
- **📱 Telegram Trade Alerts**: Instant webhook notifications directly to your phone when buy/sell conditions trigger.
- **💳 Stripe Quant Monetization**: Live pricing preview for recurring monthly subscriptions ($49/mo) and lifetime access ($149).

---

## 🏗️ Production Micro-SaaS Architecture

```
zenbot-pro/
├── prisma/
│   └── schema.prisma                # User, ExchangeKey, TradingBot, TradeOrder & BacktestRun
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── trading/
│   │   │   │   ├── market-data/route.ts  # Binance live OHLCV candlestick fetcher
│   │   │   │   └── backtest/route.ts     # Server-side backtesting engine
│   │   │   └── stripe/
│   │   │       ├── checkout/route.ts     # Stripe Checkout session creator
│   │   │       └── webhook/route.ts      # Automated plan upgrade webhook
│   │   ├── globals.css                   # High-contrast terminal styling
│   │   ├── layout.tsx                    # SEO & Root Layout
│   │   └── page.tsx                      # Complete visual quant terminal
│   ├── lib/
│   │   ├── db.ts                         # Prisma client singleton
│   │   ├── exchange/
│   │   │   └── binance.ts                # Binance REST client & HMAC-SHA256 signature
│   │   ├── strategies/
│   │   │   └── rsi_macd.ts               # Algorithmic momentum & mean-reversion
│   │   ├── notifications/
│   │   │   └── telegram.ts               # Instant buy/sell Telegram alerts
│   │   └── stripe.ts                     # Stripe plans & billing config
│   └── types/
│       └── trading.ts                    # TypeScript types for orders, tickers & candles
├── .env.example                          # Documented environment variables
├── package.json
└── README.md
```

---

## 💰 Built-in Monetization & Business Model

ZenBot Pro includes a pre-configured recurring software business model:

| Plan | Price (Global) | Price (Brazil) | Features |
| :--- | :---: | :---: | :--- |
| **Trader Starter** | $0 | R$ 0 | 1 simulation bot, standard RSI+MACD, 30-day backtesting |
| **Quant Pro Monthly** | $49 / mo | R$ 199 / mês | Up to 5 live bots, Binance & Bybit Testnet, Telegram alerts, 1-yr backtesting |
| **Lifetime Quant** | $149 once | R$ 599 único | Unlimited bots, complete TypeScript source code, zero profit fees, priority support |

---

## 🚀 Quick Start Guide (English)

### 1. Clone & Install
```bash
git clone https://github.com/KipTecnologia/zenbot-pro.git
cd zenbot-pro
npm install
```

### 2. Configure Environment Variables
```bash
cp .env.example .env
```
Add your keys:
- `DATABASE_URL`: Defaults to `file:./dev.db` for instant local setup.
- `BINANCE_API_KEY` & `BINANCE_API_SECRET`: (Optional) Free testnet keys at [testnet.binance.vision](https://testnet.binance.vision/).
- `TELEGRAM_BOT_TOKEN`: From `@BotFather` to receive instant trade notifications.
- `STRIPE_SECRET_KEY`: For monetization checkout.

### 3. Initialize Database & Run
```bash
npx prisma db push
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) to view the terminal.

---

## 🇧🇷 Guia de Início Rápido (Português)

### 1. Instalação e Execução
```bash
git clone https://github.com/KipTecnologia/zenbot-pro.git
cd zenbot-pro
npm install
cp .env.example .env
npx prisma db push
npm run dev
```

### 2. Conectar com a Binance Testnet
O projeto opera em modo seguro por padrão na rede Testnet da Binance. Basta obter credenciais gratuitas sem custos em [testnet.binance.vision](https://testnet.binance.vision/) e colar no `.env`.

---

## 🏢 About Kip Tecnologia

**ZenBot Pro** is engineered and maintained by **Kip Tecnologia**.

- **Website**: [kiptecnologia.com.br](https://kiptecnologia.com.br)
- **GitHub**: [github.com/KipTecnologia](https://github.com/KipTecnologia)
- **Support**: `contato@kiptecnologia.com.br`

---

## 💎 Commercial Licensing vs. Public Demo

| Feature / Asset | Public Interactive Demo (Free) | Commercial License & Full Boilerplate (Paid) |
| :--- | :---: | :---: |
| **Interactive Quant Terminal** | ✅ Free Access | ✅ Included |
| **Bilingual Switcher (EN / PT)** | ✅ Included | ✅ Included |
| **Visual Candlestick & Technical Indicators** | ✅ Included | ✅ Included |
| **Next.js 15 App Router Full Source** | ❌ (Commercial) | ✅ **100% Unlocked** |
| **Prisma ORM & SQLite/PostgreSQL Database** | ❌ (Commercial) | ✅ **Production Models** |
| **Binance Testnet & Live REST / HMAC Connector** | ❌ (Commercial) | ✅ **Production Integration** |
| **Telegram Signals Webhook Dispatcher** | ❌ (Commercial) | ✅ **Production Endpoints** |
| **Stripe Subscriptions & Webhook Handlers** | ❌ (Commercial) | ✅ **Turnkey Setup** |
| **100% White-Label Rights (Zero Profit Cut)** | ❌ (Evaluation only) | ✅ **Full Commercial Rights** |
| **Lifetime Updates & Discord VIP Access** | ❌ (Evaluation only) | ✅ **Included** |

👉 **[Acquire Commercial License & Full Boilerplate on Gumroad](https://rancharia.gumroad.com)**

---

## 📄 License

This repository is governed by the **Kip Tecnologia Commercial & Evaluation License (v2.0)**. The interactive demo and public assets are available for evaluation purposes. Commercial reproduction, distribution, and SaaS operation require a valid Commercial License from Kip Tecnologia. Copyright (c) 2026 Kip Tecnologia.
