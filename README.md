# 🚀 RainSure  
### AI-Powered Parametric Income Protection for Delivery Partners  

---

## 💡 Overview

RainSure is a parametric insurance platform designed specifically for food delivery partners (Swiggy/Zomato). It protects workers from **income loss caused by external disruptions** such as heavy rainfall, extreme heat, pollution, curfews, and platform outages.

Unlike traditional insurance:
- ❌ No claim forms  
- ❌ No approval delays  
- ✅ Fully automated payouts  

The system detects disruptions, validates worker inactivity, and **instantly compensates lost income**.

---

## 🎯 Core Features

### 1. 🧾 Smart Onboarding
- OTP-based login (mobile-first)
- Worker selects platform (simulated API)
- System fetches or estimates:
  - Weekly income
  - Work hours
  - Active zones
- Generates a **personalized risk profile**

---

### 2. 🤖 AI-Based Risk Profiling
The system assigns a **risk level (Low / Medium / High)** using:
- Historical weather data
- Zone-level disruption frequency
- Worker activity patterns
- Seasonal trends

👉 Output: Risk score used for pricing + fraud detection

---

### 3. 💰 Weekly Insurance Model
- Designed for gig workers’ weekly earnings cycle
- Flexible plans:
  - Lite, Plus, Max
- Dynamic pricing adjusts weekly based on:
  - Weather forecast
  - Location risk
  - Worker history

👉 Affordable micro-premiums (₹30–₹90/week)

---

### 4. 🌦️ Real-Time Monitoring Engine
Continuously tracks:
- Weather (rainfall, temperature)
- Air Quality Index (AQI)
- Government alerts (curfews, shutdowns)
- Platform availability (mock APIs)

👉 Runs every few minutes using background jobs

---

### 5. ⚡ Parametric Claim Triggering
Claims are triggered automatically when:
- A disruption crosses predefined thresholds  
- Worker is inactive during that period  

Example:
- Rainfall > 25mm/hr  
- Worker has no delivery activity  

➡️ Claim is auto-initiated (no user input)

---

### 6. 💸 Instant Payout System
- Income loss is calculated using:
  - Past earnings
  - Lost work hours
- Payment sent via:
  - UPI / Wallet (sandbox)

👉 Payout time: within minutes

---

### 7. 🛡️ Intelligent Fraud Detection
Multi-layer fraud prevention system:

#### Signals Used:
- GPS vs actual movement patterns  
- Device fingerprinting  
- Platform activity mismatch  
- Duplicate claims  
- Network inconsistencies  

#### AI Models:
- Isolation Forest (anomaly detection)
- Rule-based validation

👉 Each claim gets a **fraud risk score**

---

### 8. 🚨 Anti-Spoofing Protection
To prevent GPS spoofing attacks:

- Motion sensor validation (accelerometer, speed)
- IP location vs GPS comparison
- Crowd validation (nearby worker behavior)
- Detection of:
  - Emulator usage
  - Mock location apps

👉 Ensures only genuine workers get paid

---

### 9. 📊 Analytics Dashboard

#### Worker Dashboard:
- Active coverage
- Earnings protected
- Claim history

#### Admin Dashboard:
- Fraud alerts
- Risk zones (heatmap)
- Payout trends
- System performance

---

### 10. 🧠 AI Chatbot (Optional Feature)
- Multilingual support
- Helps users:
  - Understand policy
  - Track claims
  - Ask queries

---

## 📐 Payout Calculation Logic


---

## ⚙️ Tech Stack (Clearly Defined)

### 🔹 Frontend

| Component | Technology | Purpose |
|----------|-----------|--------|
| Mobile App | React Native (Expo) | Primary interface for workers |
| Web Dashboard | React.js + Tailwind CSS | Admin analytics panel |
| Charts | Recharts / D3.js | Data visualization |
| Maps | Leaflet.js | Zone-based tracking |

---

### 🔹 Backend

| Component | Technology | Purpose |
|----------|-----------|--------|
| API Server | FastAPI (Python) | Handles all backend logic |
| Database | PostgreSQL | Stores users, policies, claims |
| Cache | Redis | Real-time state + fast access |
| Task Queue | Celery | Background jobs (trigger monitoring) |
| Authentication | JWT + OTP | Secure login |

---

### 🔹 AI/ML Layer

| Feature | Model | Purpose |
|--------|------|--------|
| Premium Pricing | XGBoost / LightGBM | Dynamic pricing |
| Risk Forecasting | Prophet | Predict disruptions |
| Fraud Detection | Isolation Forest | Detect anomalies |
| Chatbot | LLM API + RAG | User interaction |

---

### 🔹 Integrations

| Service | API | Type |
|--------|-----|-----|
| Weather | OpenWeatherMap | Live |
| Air Quality | OpenAQ | Live |
| Payments | Razorpay | Sandbox |
| Platform Data | Mock APIs | Simulated |
| Maps | OpenStreetMap | Free |

---

### 🔹 Infrastructure

| Component | Tool |
|----------|-----|
| Cloud | AWS (EC2, RDS, S3) |
| CI/CD | GitHub Actions |
| Containers | Docker |
| Monitoring | Logs + dashboards |

---

## 🚀 Key Highlights

- Fully automated insurance (zero manual claims)
- Weekly pricing aligned with gig economy
- Real-time parametric triggers
- AI-powered fraud detection
- Mobile-first design for accessibility
- Scalable and production-ready architecture

---

## ❌ What We Do NOT Cover

- Health insurance  
- Accidents or injuries  
- Vehicle damage  
- Personal property loss  

✔ Only income loss due to external disruptions

---

## 🏁 Conclusion

RainSure reimagines insurance for gig workers by combining **AI, automation, and real-time data** to provide a fast, fair, and reliable safety net for income disruption.

It ensures that even when work stops, **earnings don’t**.
