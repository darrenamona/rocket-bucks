# 🚀 Rocket Bucks

A modern personal finance management app with real-time bank account integration powered by Plaid.

## ✨ Features

- 💰 **Real Bank Integration**: Connect actual financial institutions via Plaid
- 📊 **Transaction Tracking**: Automatically import and categorize transactions
- 💳 **Multiple Accounts**: Link checking, savings, credit cards, and investment accounts
- 📈 **Net Worth Tracking**: View all your accounts in one place
- 🤖 **AI Insights**: Get intelligent financial insights
- 🎯 **Spending Analysis**: Track and analyze your spending patterns
- 🔄 **Recurring Transactions**: Identify subscription and recurring payments

## 🏦 Production Environment

**This app is configured for Plaid's production environment** - users can connect their real bank accounts and see actual financial data from 11,000+ supported institutions.

## 🚀 Quick Start

See **[PRODUCTION_SETUP.md](./PRODUCTION_SETUP.md)** for detailed setup instructions.

### Prerequisites

- Node.js 18+ installed
- Plaid production API credentials
- Approved for Plaid production access

### Installation

1. Install dependencies:

```bash
npm install
```

2. Create `.env` file with your Plaid production credentials:

```env
# Supabase Configuration
SUPABASE_URL=...
SUPABASE_ANON_KEY=...
SUPABASE_SERVICE_ROLE_KEY=...

# Plaid Configuration
PLAID_CLIENT_ID=...
PLAID_SECRET=...
PORT=3001

# Encryption
ENCRYPTION_KEY=...

# OPENROUTER CHAT BOT
OPENROUTER_API_KEY=...

```

3. Start the application:

```bash
# Terminal 1 - Backend
npm run server

# Terminal 2 - Frontend  
npm run dev
```

4. Navigate to [http://localhost:5173](http://localhost:5173)

## 📚 Documentation

- **[PRODUCTION_SETUP.md](./PRODUCTION_SETUP.md)** - Complete production setup guide
- **[README_PLAID.md](./README_PLAID.md)** - Plaid integration details
- **[PLAID_SETUP.md](./PLAID_SETUP.md)** - Quick setup reference

## 🔐 Security

- Bank-level encryption (256-bit SSL)
- Read-only access to accounts
- Credentials never stored
- Environment variables protected via .gitignore

## 🛠️ Tech Stack

- **Frontend**: React + TypeScript + Vite + Tailwind CSS
- **Backend**: Express.js + Node.js
- **Integration**: Plaid API (Production)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).
