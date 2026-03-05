🚨 NearHelp
AI-Based Geo-Intelligent Emergency Response Platform

NearHelp is a real-time, AI-powered emergency response system that connects people in distress with nearby verified responders using geospatial intelligence, automation workflows, and conversational AI.

It is not just an SOS app — it is a crisis orchestration platform designed for faster, smarter, and community-driven emergency intervention.

🌍 Problem Statement

During emergencies:

Response time is delayed

Communication is fragmented

Panic reduces clarity

False alerts reduce system trust

Escalation processes are manual

NearHelp solves these challenges by combining real-time geolocation, AI triage, automation, and multi-channel communication into one unified system.

💡 Proposed Solution

NearHelp enables:

📍 Real-time SOS broadcasting using geospatial filtering

🧠 AI-driven emergency classification & severity scoring

🔁 Automated escalation workflows

📞 Multi-channel alerting (In-app + SMS + Voice)

🤝 Community-based responder network

🛡 Admin monitoring with fraud detection

🏗 System Architecture
1️⃣ Client Layer

Web Application (React / JS)

Leaflet for live maps

Role-based dashboards (Citizen, Responder, Admin)

2️⃣ Backend Layer (Supabase)

PostgreSQL Database

PostGIS for geospatial queries

JWT Authentication

Row-Level Security (RLS)

Realtime subscriptions

RPC function: get_nearby_sos()

3️⃣ Automation Layer (n8n)

SOS event triggers

Escalation workflows

Welfare checks

Guardian notifications

Admin alerts

4️⃣ AI & Intelligence Layer

Botpress (Conversational triage)

Severity scoring engine

Fraud detection logic

ElevenLabs (AI voice assistance)

5️⃣ Communication Layer

Supabase Realtime notifications

Twilio SMS alerts

Twilio Voice integration

🔁 End-to-End Flow

User triggers SOS

Location captured via GPS

Event stored in Supabase

Nearby responders notified via PostGIS filtering

n8n triggers AI triage

Severity assigned

If no response → automated escalation (SMS/Voice)

Admin dashboard updates in real-time

🛠 Tech Stack
Layer	Technology
Frontend	React / JavaScript / Leaflet
Backend	Supabase (PostgreSQL + PostGIS)
Authentication	Supabase Auth (JWT)
Automation	n8n
Messaging	Twilio
Conversational AI	Botpress
Voice AI	ElevenLabs
Database Security	Row Level Security (RLS)
🚀 Key Features

🔴 Real-time SOS broadcasting

📍 Radius-based emergency filtering

🧠 AI severity classification

📊 Admin analytics dashboard

🤝 Community responder network

🔐 Secure role-based access

📞 Multi-channel escalation

🌐 Scalable cloud architecture

📊 Feasibility
Technical Feasibility

Cloud-based architecture

Real-time geospatial processing

AI-driven automation

Multilingual conversational support

Operational Feasibility

Modular and scalable

Centralized admin control

Fraud detection system

Multi-city deployment ready

Economic Feasibility

Built using open-source technologies

Serverless backend model

Low infrastructure cost

Cloud-based scalability

⚠ Challenges & Mitigation
Challenge	Strategy
Data Privacy	Encryption + RLS + Secure JWT
AI Accuracy	Continuous model training
User Adoption	Simple UI + awareness programs
Connectivity Issues	SMS fallback escalation
False Alerts	AI fraud detection
🥚 Easter Eggs

NearHelp includes two hidden interactive surprises built into the AI and voice layers:

🎤 Voice Trigger Easter Egg

If you loudly say “OJASS for NIT-JSR” and sharply shout “NITJSR!”, the system activates a special hidden response within the voice interaction module.

Location: Voice AI Interaction (ElevenLabs Integration)

🤖 Bot Intelligence Easter Egg

If you ask the ElevenLabs bot:
“What is OJASS?”

The bot delivers a custom hidden response designed exclusively for OJASS at NIT-JSR.

Location: Conversational AI Layer (Botpress + ElevenLabs Response Logic)

🎯 Future Enhancements

Guardian live tracking

Heatmap-based emergency analytics

Predictive risk modeling

Authority integration APIs

Mobile app deployment

Multi-language expansion

📌 Why NearHelp?

NearHelp transforms emergency response from a reactive system into a proactive, AI-powered crisis management network.

It combines:

Real-time geospatial intelligence

Automated escalation workflows

Conversational AI support

Community-driven assistance

To deliver faster, smarter, and safer emergency intervention.

🏆 Built For

Hack De Science (OJASS-2026)

👥 Team

Developed by Team Null Pointers with a focus on scalable architecture, secure backend systems, and intelligent automation workflows.

📄 License

This project is developed for educational and innovation purposes.

