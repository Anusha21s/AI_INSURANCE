# 🛵 RiderNet

## ₹140.

That’s what Karthik earned last Wednesday.

He planned for ₹700.
School fees were due Friday.
His bike EMI hits on the 5th.

The rain didn’t care.
The app didn’t care.
No insurance product cared.

**We did.**

---

#  Who is our user?

RiderNet is built for gig delivery partners — but not all riders are the same.

### 1. Full-Time Rider (Karthik)

* Depends completely on delivery income
* Highly affected by weather disruptions

### 2. Part-Time Rider (Student / Freelancer)

* Works during peak hours
* Needs flexible and affordable protection

### 3. Rural / Semi-Urban Rider

* Faces GPS inaccuracies
* Has unstable internet connectivity

 RiderNet ensures fairness and protection across all these personas.

---

#  Problem Statement

Delivery partners face:

* No income during disruptions
* No protection for lost wages
* No formal financial safety net

## Existing Systems Fail

| System            | Limitation                       |
| ----------------- | -------------------------------- |
| Health Insurance  | Covers injuries, not income loss |
| Vehicle Insurance | Covers damage, not earnings      |
| Platforms         | No downtime compensation         |
| Loans             | Increase debt                    |

---

#  Our Solution — RiderNet

**Parametric Income Protection for Gig Workers**

Automatic payouts triggered by real-world conditions — no claims, no delays.

---

#  Smart Payout Triggers

| Condition              | Payout  |
| ---------------------- | ------- |
| Rain > 64.4 mm         | Full    |
| Heat > 45°C            | 50%     |
| AQI > 400              | Partial |
| Flood (Govt confirmed) | Full    |
| Bandh (Verified)       | Full    |

---

#  Adversarial Defense & Anti-Spoofing Strategy

## The Attack

500 fake riders → Fake GPS → Real payouts → System drained

**Core Problem:**
Parametric systems trust data, not presence.

---

##  Multi-Layer Defense System

### Layer 1 — GPS & Physics Validation

GPS can be faked. Physics cannot.

We detect:

* Teleportation (>5 km jump)
* Unrealistic speeds (>40 km/h in rain)
* No movement for long durations
* Abnormal altitude changes

 3 violations → claim blocked

Also includes:

* Mock GPS detection
* Device fingerprinting

---

### Layer 2 — Behavioral Analysis

| Signal        | Real Rider | Fraud        |
| ------------- | ---------- | ------------ |
| Past activity | Consistent | None         |
| Zone presence | Stable     | Random       |
| Work pattern  | Continuous | Trigger-only |

 New accounts → capped at 50% payout

---

### Layer 3 — Claim Pattern Detection

* Real events → gradual claim distribution
* Fraud → sudden spikes (e.g., 400 claims in minutes)

 Action: Temporary hold + verification

---

### Layer 4 — Multi-Signal Verification

We require **3 out of 5 signals**:

* GPS
* Cellular tower
* Order activity
* Weather data
* Historical presence

 Fraud fails
 Genuine riders pass smoothly

---

### Layer 5 — Fraud Ring Detection

We construct a **claim graph**:

* Nodes → claims
* Edges → shared device / IP / UPI

 Detects coordinated fraud networks, not just individuals

---

### Layer 6 — Fairness & Risk Scoring

| Score  | Action         |
| ------ | -------------- |
| 0–30   | Instant payout |
| 31–60  | Partial payout |
| 61–80  | Manual review  |
| 81–100 | Block + appeal |

## Rider Protection Mechanisms

* Appeal system (video proof)
* Rural flexibility (2/5 signals allowed)
* Trust score boost after false flags

 Genuine riders like Karthik show consistent behavior and pass verification without friction.

---

#  How Our AI Works

* **XGBoost** → Calculates premium based on:

  * Weather risk
  * Rider history
  * Location risk

* **Isolation Forest** → Detects anomalies such as:

  * Fake GPS patterns
  * Sudden claim spikes
  * Unusual behavior

* **Prophet** → Forecasts:

  * Weather disruptions
  * High-risk periods

 Together, they form a **predictive + defensive AI system**.

---

#  System Architecture

1. Rider app sends GPS, device, and activity data
2. Backend validates multi-signal inputs
3. AI models analyze risk & fraud probability
4. Decision engine evaluates claim
5. Payout triggered instantly or flagged

---

#  Pricing Model

Weekly subscription aligned with rider income

Base: ₹29 + Risk Score Adjustment

Example: ₹74.50/week

---

##  Plans

| Tier     | Price | Coverage |
| -------- | ----- | -------- |
| Basic    | ₹29   | ₹500     |
| Standard | ₹49   | ₹750     |
| Premium  | ₹79   | ₹900     |

---

#  App Features

* Multi-language UI
* 2-minute onboarding
* Real-time alerts
* Earnings dashboard

###  Rainy Day Mode

UI adapts emotionally during disruptions

---

#  Tech Stack

### Frontend

* React + Vite
* TailwindCSS

### Backend

* FastAPI
* PostgreSQL

### AI/ML

* XGBoost
* Isolation Forest
* Prophet

### APIs

* OpenWeatherMap
* OpenAQ
* NewsAPI

---

#  Why RiderNet is Different

* Not traditional insurance → **real-time income protection**
* Not GPS-dependent → **multi-signal verification system**
* Not reactive → **predictive AI-driven system**
* Not individual-focused → **fraud network detection**

---

#  Workflow

1. Rider registers
2. Premium calculated dynamically
3. Event detected
4. Fraud checks executed
5. Payout processed

---

#  Status

Phase 1 — Ideation

* Problem validated
* System designed
* Prototype in progress

---

#  Team

Bannari Amman Institute of Technology, Erode

* Anusha S — Full Stack
* Abinaya S — Backend & ML
* Jeyashri M — UI/UX
* Kamalikaa K — Data

---

#  Final Thought

Friday morning.
School fees paid.
Family okay.

That’s not a feature.
That’s the goal.

---

## 🛵 RiderNet

**Because no rider should lose income to the weather.**
