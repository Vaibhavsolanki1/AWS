# JanSaarthi AI — Requirements Document

## 1. Project Overview

JanSaarthi AI is a multilingual, voice-first AI assistant designed to help citizens discover and access government schemes easily. The system provides personalized scheme recommendations, eligibility checks, application guidance, and documentation support.

The goal is to reduce the access gap caused by:

* Lack of awareness
* Complex eligibility rules
* Language barriers
* Poor digital literacy
* Fragmented government platforms

---

## 2. Functional Requirements

### 2.1 User Interaction

The system must allow users to:

* Speak or type queries
* Select preferred language
* Provide personal profile details
* Receive scheme recommendations
* Download a personalized report (PDF)

---

### 2.2 Scheme Discovery

The system must:

* Suggest relevant government schemes
* Filter schemes using user profile
* Support geo-location filtering
* Display documentation requirements
* Provide application steps

---

### 2.3 Eligibility Engine

The system must:

* Evaluate eligibility using rule-based logic
* Provide instant eligibility feedback
* Explain why a user qualifies or not

---

### 2.4 Voice and Language Support

The system must:

* Support multilingual interaction (10+ Indian languages)
* Convert speech to text
* Convert responses to speech

---

### 2.5 Communication Channels

The system must support:

* Android application
* WhatsApp chatbot
* IVR interface

---

## 3. Non-Functional Requirements

### Performance

* Response time under 3 seconds
* Optimized for low bandwidth environments

### Scalability

* Support up to 1M users
* Modular service architecture

### Security

* Secure user data storage
* HTTPS communication
* Authentication for admin access

### Reliability

* 99% uptime target
* Fault-tolerant backend services

---

## 4. Data Requirements

### Government Scheme Database

Must store:

* Scheme name
* Eligibility criteria
* Required documents
* Application steps
* Region applicability

---

### User Profile Data

May include:

* Age
* Occupation
* Income range
* Location
* Education level

---

## 5. Future Requirements

* Fraud detection module
* NGO collaboration dashboard
* Government analytics dashboard

---

## 6. Success Metrics

* Number of users onboarded
* Eligibility checks performed
* Schemes successfully discovered
* Report downloads
* Regional adoption rate
