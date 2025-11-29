# 🚀 Uptime-Lite

**Uptime-Lite** is an open-source, developer-first uptime monitoring and status graph platform that can be integrated into any application in just **2–4 simple steps**. It provides real-time uptime checks, response time monitoring, beautiful graphs, and a public status page — with both **self-hosted** and **cloud-ready** support.

> **One-line vision:** Add uptime monitoring to any app in under 60 seconds.

---

## ✨ Key Features

* ✅ Simple 2–4 step integration
* ✅ Real-time uptime monitoring
* ✅ Response time tracking
* ✅ Automatic status graphs (24h / 7d)
* ✅ Public status page per project
* ✅ API-key based project system
* ✅ Lightweight JavaScript SDK
* ✅ Self-hosted with Docker
* ✅ Open-source & community-driven

---

## 🎯 Who Is This For?

* Indie developers
* Startup teams
* SaaS builders
* DevOps & SRE engineers
* Open-source maintainers

If you run APIs, websites, or microservices — Uptime-Lite fits right in.

---

## ⚡ 2–4 Step Integration (Developer Experience)

### ✅ Step 1: Install SDK

```bash
npm install uptime-lite
```

---

### ✅ Step 2: Initialize

```js
import { initUptime } from "uptime-lite";

initUptime({
  apiKey: "YOUR_PROJECT_API_KEY",
  appName: "My Production API"
});
```

---

### ✅ Step 3: Register Endpoint

```js
monitor("https://api.myapp.com/health");
```

🎉 Done! Your service is now live on the dashboard.

---

### ✅ Optional Step 4: Custom Ping

```js
ping("auth-service");
```

---

## 🏗️ System Architecture

```
Developer App
     │
     ▼
SDK → Backend API → Worker → Target URL
                    │
                    ▼
                 Database
                    │
                    ▼
               Dashboard UI
```

### Components

* **SDK:** Sends heartbeat and monitor requests
* **Backend API:** Handles projects, keys, and endpoints
* **Worker:** Periodically checks URLs
* **Database:** Stores uptime logs and metrics
* **Dashboard UI:** Displays graphs and current status

---

## 🛠️ Tech Stack

### Backend

* Node.js
* Express.js
* Prisma ORM

### Database

* PostgreSQL or MongoDB

### Worker

* node-cron
* Axios / Fetch

### Frontend Dashboard

* Next.js or React
* Chart.js / Recharts

### DevOps & Deployment

* Docker
* Docker Compose
* NGINX
* GitHub Actions

---

## ✅ MVP Feature Scope

### Core Features (v1)

* Project and API key system
* URL uptime monitoring
* Response time logging
* Failure & success records
* 24h & 7-day graphs
* Public status page
* JavaScript SDK

### Planned Features (v2+)

* Email & Discord alerts
* Slack & webhook integrations
* Multi-region monitoring
* Status badges for GitHub
* Incident tracking
* Maintenance windows

---

## 📁 Repository Structure

```
uptime-lite/
 ├── apps/
 │    ├── api/
 │    ├── worker/
 │    ├── dashboard/
 │
 ├── sdk/
 ├── docs/
 ├── docker-compose.yml
 ├── README.md
 └── LICENSE
```

---

## 🚀 Getting Started (Local Setup)

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-org/uptime-lite.git
cd uptime-lite
```

---

### 2️⃣ Setup Environment

```bash
cp .env.example .env
```

Add database and API secrets.

---

### 3️⃣ Start With Docker

```bash
docker-compose up -d
```

---

### 4️⃣ Open Dashboard

```
http://localhost:3000
```

---

## 🌍 Public Status Page

Each project automatically generates a public page:

```
https://status.yourdomain.com/project-id
```

It shows:

* Current uptime
* Outage history
* Performance graphs

---

## 🔐 Security

* API keys per project
* Rate-limited public endpoints
* No sensitive payload storage
* HTTPS-ready deployment

---

## 🧠 Open-Source Philosophy

Uptime-Lite is built with:

* Transparency
* Easy self-hosting
* Minimal vendor lock-in
* Community contributions

---

## 🤝 Contribution Guidelines

We welcome contributions!

1. Fork the repo
2. Create your feature branch
3. Commit your changes
4. Open a pull request

Please follow clean code practices and include tests where possible.

---

## 📜 License

MIT License — free to use, modify, and distribute.

---

## 🌟 Roadmap

* ✅ MVP with core uptime monitoring
* ⏳ Hosted SaaS version
* ⏳ Multi-region monitoring
* ⏳ Status badges
* ⏳ Incident management

---

## 📬 Contact & Community

* GitHub Issues & Discussions
* Future Discord community (coming soon)

---

🔥 **Uptime-Lite — Simple uptime. Powerful insight. Open-source forever.**

# result and get result of downtime

#Service: Payment API
Deployment: v2.4.1
Status: DOWN
Detected Cause: MongoDB connection timeout

Last 10 Logs:
--------------------------------
Error: MongoNetworkError
at connect (/src/db.js:45)

Crash Time: 10:31 AM IST
--------------------------------

