# RainSure  
AI-Powered Parametric Income Protection for Food Delivery Partners  

"When work stops due to external disruptions, your income shouldn’t."

---

## Overview

RainSure is an AI-enabled parametric insurance platform designed for food delivery partners working with platforms like Swiggy and Zomato. The platform protects workers from income loss caused by external disruptions such as extreme weather, pollution, curfews, and platform outages.

Unlike traditional insurance systems, RainSure operates without manual claims. It detects disruption events in real time, validates income loss using data signals, and triggers instant payouts.

RainSure strictly focuses on income protection and does not cover health, life, accidents, or vehicle damage.

---

## Persona: Food Delivery Partner

### Profile

Example: Ravi, a 26-year-old delivery partner in Chennai  
- Works 9–11 hours daily  
- Earns ₹500–₹900 per day  
- Paid weekly  
- Operates in a 5–8 km delivery zone  

### Key Characteristics

- Weekly income: ₹3,000–₹6,000  
- Highly dependent on weather and demand  
- Works in localized zones  
- Smartphone-first user  
- Requires simple, low-friction interfaces  
- No financial safety net during disruptions  

---

## Disruption Scenarios

| Scenario | Trigger | Impact |
|----------|--------|--------|
| Heavy Rainfall | Rainfall > 30mm/hr | Significant drop in orders |
| Extreme Heat | Temperature > 42°C | Reduced delivery activity |
| Severe Pollution | AQI > 300 | Health advisories limit work |
| Curfew / Shutdown | Government or news alerts | Complete halt of operations |
| Platform Outage | Downtime > 60 minutes | No order availability |

---

## Application Workflow

1. Onboarding  
   Worker registers via mobile app using OTP authentication  
   Connects delivery platform (simulated integration)  
   System analyzes past earnings and work patterns  

2. Risk Profiling  
   AI model assigns a risk score based on zone and behavior  

3. Policy Purchase  
   Worker selects a weekly plan and completes payment  
   Policy activates for the current or upcoming cycle  

4. Real-Time Monitoring  
   System continuously monitors weather, AQI, and external signals  

5. Parametric Trigger  
   If disruption conditions are met and worker activity drops, claim is auto-triggered  

6. Payout  
   Income loss is calculated and payout is sent instantly via UPI  

7. Dashboard  
   Workers and admins can view analytics, claims, and system insights  

---

## Weekly Premium Pricing Model

RainSure follows a weekly subscription model aligned with gig worker income cycles.

### Plans

| Plan | Weekly Premium | Max Weekly Payout | Coverage |
|------|--------------|------------------|----------|
| Lite | ₹30 | ₹300 | Limited hours |
| Plus | ₹60 | ₹700 | Moderate coverage |
| Max | ₹90 | ₹1200 | Full coverage |

---

### Dynamic Pricing Factors

| Factor | Effect |
|--------|--------|
| Weather forecast severity | ±20% |
| Zone disruption history | ±15% |
| City risk level | ±25% |
| Worker activity consistency | ±10% |

---

## Payout Calculation

---

## Parametric Triggers

| Trigger | Data Source | Threshold |
|--------|-------------|----------|
| Rainfall | Weather API | >25mm/hr |
| Heat Index | Weather API | >44°C |
| Air Quality | OpenAQ API | AQI >300 |
| Curfew | News/NLP signals | Confirmed event |
| Platform Downtime | Mock API | >60 minutes |

All triggers are location-specific and validated at zone level.

---

## AI/ML Integration

### 1. Premium Pricing Model
- Algorithm: Gradient Boosting (XGBoost / LightGBM)  
- Inputs: weather history, claims data, worker behavior  
- Output: weekly premium multiplier  

### 2. Risk Forecasting
- Model: Time-series forecasting (Prophet)  
- Predicts disruption probability for upcoming days  

### 3. Fraud Detection
- Model: Isolation Forest + rule-based checks  
- Detects abnormal patterns in claims and behavior  

### 4. Chatbot Support
- LLM-based assistant for onboarding and support  
- Multilingual interaction  

---

## Adversarial Defense and Anti-Spoofing Strategy

### Differentiation Approach

The system does not rely solely on GPS. It validates claims using behavioral, environmental, and device-level signals.

A genuine worker shows:
- Continuous movement history  
- Gradual activity drop during disruption  
- Alignment with environmental conditions  

A spoofed user shows:
- Sudden location jumps  
- No prior activity in the zone  
- Inconsistent behavior patterns  

---

### Data Signals Used

Movement Data  
- Route continuity  
- Speed and motion patterns  

Network Data  
- Signal fluctuation  
- IP location consistency  

Device Data  
- Mock GPS detection  
- Emulator or rooted device detection  

Crowd Intelligence  
- Nearby worker activity comparison  
- Detection of coordinated claim clusters  

Environmental Validation  
- Cross-check between disruption intensity and worker inactivity  

---

### Fraud Scoring and UX Balance

| Risk Level | Action |
|------------|--------|
| Low | Instant payout |
| Medium | Lightweight verification |
| High | Manual review |

The system ensures minimal friction for genuine users while preventing large-scale fraud.

---

## Features Summary

- Automated onboarding with minimal input  
- AI-driven risk profiling  
- Weekly flexible pricing model  
- Real-time disruption monitoring  
- Zero-claim parametric insurance system  
- Instant payout mechanism  
- Multi-layer fraud detection  
- Anti-spoofing protection  
- Worker and admin dashboards  
- Scalable architecture  

---

## Tech Stack

### Frontend

| Component | Technology |
|----------|-----------|
| Mobile App | React Native (Expo) |
| Web Dashboard | React.js + Tailwind CSS |
| Charts | Recharts / D3.js |
| Maps | Leaflet.js |

---

### Backend

| Component | Technology |
|----------|-----------|
| API Server | FastAPI (Python) |
| Database | PostgreSQL |
| Cache | Redis |
| Task Queue | Celery |
| Authentication | JWT + OTP |

---

### AI/ML

| Component | Technology |
|----------|-----------|
| Pricing Model | XGBoost / LightGBM |
| Risk Forecasting | Prophet |
| Fraud Detection | Isolation Forest |
| Chatbot | LLM API + RAG |

---

### Integrations

| Service | API |
|--------|-----|
| Weather | OpenWeatherMap |
| Air Quality | OpenAQ |
| Payments | Razorpay (sandbox) |
| Platform Data | Mock APIs |
| Maps | OpenStreetMap |

---

### Infrastructure

- AWS (EC2, RDS, S3)  
- Docker and Docker Compose  
- GitHub Actions (CI/CD)  
- Logging and monitoring (basic setup)  

---

## Development Plan

### Phase 1: Ideation and Foundation
- Define persona and problem  
- Design pricing and triggers  
- Setup repository and architecture  
- Create UI wireframes  

### Phase 2: Core System Development
- Implement onboarding and policies  
- Integrate parametric triggers  
- Build claim automation system  
- Develop fraud detection engine  

### Phase 3: Optimization and Scaling
- Improve ML models  
- Build dashboards  
- Enhance fraud prevention  
- Prepare final demo  

---

## Platform Justification

| Platform | Reason |
|----------|--------|
| Mobile | Primary interface for delivery workers |
| Web | Admin analytics and monitoring |
| Backend API | Shared services for both platforms |

---

## What We Do Not Cover

- Health insurance  
- Life insurance  
- Accident-related claims  
- Vehicle repair costs  
- Personal or asset loss  

The system strictly focuses on income loss due to external disruptions.

---

## Team

Team Name: Trio
University: Amrita Vishwa Vidyapeetham  

Members:  
- W. Venkat Ashrith
- K. Madhuri 
- M. Snigdha

---

## Links

GitHub Repository: (add link)  
Demo Video: (add link)  
Figma Wireframes: (add link)  

---

## Conclusion

RainSure introduces a new approach to insurance for gig workers by combining automation, real-time data, and AI-driven decision-making. It ensures that delivery partners are financially protected against disruptions beyond their control, providing stability in an otherwise unpredictable work environment.
