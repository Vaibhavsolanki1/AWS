# JanSaarthi AI — System Design Document

## 1. System Architecture

The system follows a modular AI-assisted service architecture.

Components:

* Android App
* WhatsApp Bot
* IVR System
* AI / NLP Engine
* Eligibility Engine
* Government Scheme Database

---

## 2. High-Level Architecture Flow

User → Interface Layer → AI/NLP → Eligibility Engine → Scheme DB → Response Generator → User

---

## 3. Component Design

### 3.1 Interface Layer

Handles user communication.

Includes:

* Android mobile app
* WhatsApp chatbot integration
* IVR voice system

Responsibilities:

* Collect user input
* Display responses
* Language selection

---

### 3.2 AI / NLP Engine

Processes user intent and language.

Responsibilities:

* Intent detection
* Entity extraction
* Language translation
* Response formatting

Possible tools:

* OpenAI / LLM APIs
* Speech-to-Text service
* Text-to-Speech service

---

### 3.3 Eligibility Engine

Rule-based evaluation system.

Responsibilities:

* Apply scheme eligibility rules
* Match user profile to schemes
* Return eligibility status

Implementation options:

* JSON rule engine
* Decision tree logic
* Python rule processor

---

### 3.4 Government Scheme Database

Central repository of schemes.

Database type:

* PostgreSQL or MongoDB

Tables/Collections:

* schemes
* eligibility_rules
* documents_required
* regions

---

### 3.5 Report Generator

Creates downloadable summary for users.

Output:

* Personalized PDF report

Includes:

* Eligible schemes
* Application steps
* Required documents

---

## 4. API Design

Example endpoints:

GET /schemes
POST /check-eligibility
POST /user-profile
GET /report
POST /voice-query

---

## 5. Deployment Design

Suggested stack:

Frontend:

* Flutter or React Native (Android)

Backend:

* Node.js / Python (FastAPI)

Database:

* PostgreSQL

AI Layer:

* LLM API
* Speech services

Hosting:

* AWS / GCP / Azure

---

## 6. Scalability Strategy

* Stateless backend services
* Load balancer
* Database indexing
* Caching layer (Redis)

---

## 7. Security Design

* Encrypted communication (HTTPS)
* Token-based authentication
* Minimal personal data storage
* Secure API gateway

---

## 8. Future Design Extensions

* Analytics dashboard
* Fraud detection AI module
* NGO integration APIs
* Offline mode support
