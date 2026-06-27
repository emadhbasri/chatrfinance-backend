# ⚙️ ChatrFinance - Backend API

> **Private Repository** · Source code is proprietary and not publicly available.

![Node.js](https://img.shields.io/badge/Node.js-20.x-339933?style=flat&logo=node.js)
![Express](https://img.shields.io/badge/Express-4.x-000000?style=flat&logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-6.x-47A248?style=flat&logo=mongodb)
![WebSocket](https://img.shields.io/badge/WebSocket-Socket.io-010101?style=flat&logo=socket.io)
![Status](https://img.shields.io/badge/Status-Production-success?style=flat)

---

## 📖 About The Project

**ChatrFinance Backend** powers the entire real-time financial data platform.

This API server handles:

- 📊 **Data Aggregation** — Fetches prices from multiple external APIs
- 🔄 **Real-time Streaming** — WebSocket server for live price updates
- 👤 **User Management** — Authentication, profiles, and roles
- ✅ **Analyst Verification** — Admin approval system for verified analysts
- 📝 **Content Management** — News feed and analyst posts in Persian
- 🗄️ **Data Persistence** — MongoDB for users, posts, and configurations
- ⏰ **Scheduled Jobs** — Cron tasks for price updates and cache refresh

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Runtime | Node.js 20.x |
| Framework | Express 4.x |
| Database | MongoDB 6.x (Mongoose ODM) |
| Real-time | Socket.io (WebSocket) |
| External APIs | Multiple financial data providers |
| Auth | JWT (JSON Web Tokens) |
| Scheduling | node-cron |
| Env Management | dotenv |

---

## 📦 Key Features

### 🔹 RESTful API Endpoints
- `GET /api/prices` — Get all current prices
- `GET /api/prices/:market` — Get specific market data
- `POST /api/auth/*` — Authentication routes
- `CRUD /api/posts` — News and analyst content
- `Admin /api/admin/*` — Verification & management

### 🔹 WebSocket Events
- `price:update` — Real-time price broadcasts
- `news:new` — New news alert
- `analyst:post` — New analyst insight

### 🔹 External Integrations
- Gold & Currency APIs (Iranian market)
- Cryptocurrency APIs (CoinGecko, etc.)
- Global stock APIs (Alpha Vantage, Yahoo Finance)
- Forex Factory news feed

### 🔹 Security & Validation
- JWT-based authentication
- Role-based access (user, analyst, admin)
- Input sanitization & validation
- Rate limiting

---

## 🚀 Quick Start (for local development)

> ⚠️ **Note:** This is a private repository. The following is for reference only.

```bash
# Clone the repo (private)
git clone [repository-url]

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your API keys and DB credentials

# Start development server
npm run dev

# Start production server
npm start