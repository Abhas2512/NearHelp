# 🚨 NearHelp
## AI-Based Geo-Intelligent Emergency Response Platform

**NearHelp** is a real-time, AI-powered emergency response platform that connects people in distress with **nearby verified responders** using **geospatial intelligence, automation workflows, and conversational AI**.

It is not just an SOS application — it is a **crisis orchestration platform** designed to enable **faster, smarter, and community-driven emergency response**.

---

# 🌍 Problem Statement

During emergencies, several critical challenges arise:

- ⏳ Delayed response time
- 📞 Fragmented communication
- 😰 Panic reduces clarity
- ⚠️ False alerts reduce trust in the system
- 🔄 Manual escalation processes

Traditional emergency systems often fail to **coordinate responders efficiently**, especially during the **first few critical minutes** of an emergency.

---

# 💡 Proposed Solution

NearHelp addresses these challenges by integrating **geolocation intelligence, AI triage, automation workflows, and multi-channel communication** into a unified system.

The platform enables:

- 📍 Real-time SOS broadcasting using geospatial filtering
- 🧠 AI-driven emergency classification & severity scoring
- 🔁 Automated escalation workflows
- 📞 Multi-channel alerting (In-App + SMS + Voice)
- 🤝 Community-based responder network
- 🛡 Admin monitoring with fraud detection

---

# 🏗 System Architecture

NearHelp follows a **multi-layer architecture** designed for scalability and real-time performance.

---

## 1️⃣ Client Layer

Handles all **user interactions and interface elements**.

### Components

- Web Application (React / JavaScript)
- Interactive map system using **Leaflet**
- Role-based dashboards

### User Roles

- Citizen (SOS sender)
- Responder (nearby helper)
- Admin (system monitoring)

---

## 2️⃣ Backend Layer (Supabase)

Acts as the **central data and authentication layer**.

### Technologies

- PostgreSQL Database
- PostGIS for geospatial queries
- Supabase Authentication (JWT)
- Row-Level Security (RLS)
- Realtime subscriptions

### Core Function

```sql
get_nearby_sos()
```
## 3️⃣ Automation Layer (n8n)

Handles **event-driven workflows and automation logic**.

### Automations include

- SOS event triggers  
- Escalation workflows  
- Welfare checks  
- Guardian notifications  
- Admin alerts  

This ensures **no SOS remains unanswered**.

---

## 4️⃣ AI & Intelligence Layer

Provides **intelligent decision-making and automated interaction**.

### Technologies

- **Botpress** → Conversational triage bot  
- **Severity Scoring Engine**  
- **Fraud Detection Logic**  
- **ElevenLabs** → AI voice assistance  

AI evaluates the emergency and determines the **urgency level and escalation strategy**.

---

## 5️⃣ Communication Layer

Ensures reliable **multi-channel emergency alerts**.

### Technologies

- Supabase Realtime Notifications  
- Twilio SMS Alerts  
- Twilio Voice Integration  

This guarantees alerts are delivered **even if the app is inactive**.

---

# 🔁 NearHelp Application Workflow

The NearHelp system follows a **real-time intelligent response pipeline**.

---

## Step 1 — SOS Trigger

A user activates the **SOS button** within the application.

- GPS location is automatically captured  
- Emergency details are recorded  

---

## Step 2 — Event Creation

The SOS request is stored in **Supabase database** with:

- User ID  
- Location coordinates  
- Timestamp  
- Emergency description  

---

## Step 3 — Geospatial Filtering

Using **PostGIS queries**, the system identifies **nearby responders within a predefined radius**.

Example query:

```sql
SELECT responders
WHERE distance < emergency_radius;
```

## Step 4 — Real-Time Notifications

Nearby responders instantly receive alerts via:

- In-app notifications  
- Realtime updates  

---

## Step 5 — AI Emergency Triage

The AI system evaluates the emergency through:

- Conversational triage (Botpress)  
- Severity classification  

The emergency receives a **severity score**.

Example categories:

- Low  
- Medium  
- High  
- Critical  

---

## Step 6 — Automated Escalation

If no responder accepts the SOS within a defined time window:

**n8n automation triggers escalation**

Actions may include:

- SMS alerts via Twilio  
- Voice calls via Twilio  
- Guardian notifications  
- Admin alerts  

---

## Step 7 — Responder Assistance

Once a responder accepts:

- Live location tracking is enabled  
- Direct communication becomes available  

---

## Step 8 — Admin Monitoring

Admins can monitor:

- Active emergencies  
- Responder activity  
- Potential fraudulent alerts  

All updates occur in **real-time dashboards**.

---

# 🚀 Key Features

- 🔴 Real-time SOS broadcasting  
- 📍 Radius-based emergency filtering  
- 🧠 AI severity classification  
- 📊 Admin analytics dashboard  
- 🤝 Community responder network  
- 🔐 Secure role-based access  
- 📞 Multi-channel escalation  
- 🌐 Scalable cloud architecture  

---

# 📊 Feasibility Analysis

## Technical Feasibility

- Cloud-native architecture  
- Real-time geospatial processing  
- AI-driven automation workflows  
- Multilingual conversational support  

---

## Operational Feasibility

- Modular and scalable system  
- Centralized admin control  
- Built-in fraud detection  
- Ready for multi-city deployment  

---

## Economic Feasibility

- Built primarily on open-source technologies  
- Serverless backend architecture  
- Minimal infrastructure requirements  
- Cloud-based scalability

---

# ⚠ Challenges & Mitigation

| Challenge | Strategy |
|----------|----------|
| Data Privacy | Encryption + RLS + Secure JWT |
| AI Accuracy | Continuous model training |
| User Adoption | Simple UI + awareness programs |
| Connectivity Issues | SMS fallback escalation |
| False Alerts | AI fraud detection |

---

# 🎯 Future Enhancements

Planned improvements for the NearHelp platform include:

- 📍 Guardian live tracking  
- 🔥 Emergency heatmap analytics  
- 🧠 Predictive risk modeling  
- 🏛 Integration with authorities  
- 📱 Native mobile application  
- 🌍 Multi-language support  

---

# 📌 Why NearHelp?

NearHelp transforms emergency response from a **reactive system into a proactive, AI-powered crisis management network**.

By combining:

- Real-time geospatial intelligence  
- Automated escalation workflows  
- Conversational AI support  
- Community-driven responders  

NearHelp delivers **faster, smarter, and safer emergency intervention**.

---
