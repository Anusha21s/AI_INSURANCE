
🛵 RiderNet

₹140.
That's what Karthik earned last Wednesday.
He planned for ₹700.
School fees were due Friday.
His bike EMI hits on the 5th.
The rain didn’t care.
The app didn’t care.
No insurance product cared.
We did.

He keeps the city fed.
The city never kept him safe.
Until RiderNet.

About This Project
This is not a typical README.
This is the story of Karthik, a delivery partner — and the system that should have protected him.
Every feature in RiderNet answers one question:
“Does this actually help the rider?”

Problem Statement
Delivery partners face:
No income during disruptions
No protection for lost wages
No formal financial safety net

Existing Systems Fail

| System            | Limitation                       |
| ----------------- | -------------------------------- |
| Health Insurance  | Covers injuries, not income loss |
| Vehicle Insurance | Covers damage, not earnings      |
| Platforms         | No downtime compensation         |
| Loans             | Increase debt                    |


Our Solution — RiderNet
Parametric Income Protection for Gig Workers
Automatic payouts triggered by real-world events.

Smart Payout Triggers
| Trigger  | Condition      | Payout  |
| -------- | -------------- | ------- |
| Rain     | > 64.4mm       | Full    |
| Heat     | > 45°C         | 50%     |
| AQI      | > 400          | Partial |
| Flood    | Govt confirmed | Full    |
| Bandh    | Verified       | Full    |



Adversarial Defense & Anti-Spoofing Strategy
The Attack
500 fake riders → Fake GPS → Real payouts → System drained

Core Problem:
Parametric insurance pays on data, not presence

Our Multi-Layer Defense System

Layer 1 — GPS & Physics Validation
GPS can be faked. Physics cannot.
We detect:
  Teleportation (>5 km jump)
  Unrealistic speeds (>40 km/h in rain)
  No movement for long durations
  Abnormal altitude changes
3 violations → Claim blocked

Also:
  Mock GPS detection (isFromMockProvider)
  Device fingerprint tracking

Layer 2 — Behaviour Analysis
We compare:
| Signal        | Real Rider | Fraud        |
| ------------- | ---------- | ------------ |
| Past activity | Regular    | None         |
| Zone presence | Consistent | Random       |
| Work pattern  | Continuous | Trigger-only |


New accounts → 50% payout cap

Layer 3 — Claim Pattern Detection
Real events → smooth claim distribution
Fraud → sudden spike (e.g., 400 claims in minutes)
Action: Temporary hold + verification

Layer 4 — Multi-Signal Verification
We require 3 out of 5 signals:
  GPS
  Cellular tower
  Order activity
  Weather data
  Historical presence
Fraud fails
  Karthik passes → gets paid instantly

Layer 5 — Fraud Ring Detection
  We build a claim graph:
    Nodes = claims
    Edges = shared data (device, IP, UPI)
  Detect entire fraud networks, not individuals

Layer 6 — Fairness & Risk Scoring

| Score  | Action           |
| ------ | ---------------- |
| 0–30   | Instant payout   |
| 31–60  | Partial payout   |
| 61–80  | Review           |
| 81–100 | Block + appeal   |


Rider Protection
  Appeal system (video proof)
  Rural flexibility (2/5 signals)
  Trust boost after false flags

Pricing Model
  Weekly -- aligned with rider income
  ₹29 + Risk Score Adjustment
  Example: ₹74.50/week
| Tier        | Price | Coverage |
| ----------- | ----- | -------- |
|    Basic    | ₹29   | ₹500     |
|    Standard | ₹49   | ₹750     |
|    Premium  | ₹79   | ₹900     |

AI/ML Engine

| System          | Tech             | Role              |
| --------------- | ---------------- | ----------------- |
| Premium Engine  | XGBoost          | Pricing           |
| Fraud Detection | Isolation Forest | Anomaly detection |
| Forecasting     | Prophet          | Risk prediction   |


Workflow
  1. Rider registers
  2. Premium calculated
  3. Event detected
  4. Fraud checks run
  5. Payout processed


App Features
  Multi-language UI
  2-min onboarding
  Real-time alerts
  Earnings dashboard
  Rainy Day Mode
  UI adapts emotionally during disruptions

Tech Stack
  Frontend
  React + Vite
  TailwindCSS
  Backend
  FastAPI
  PostgreSQL
  AI/ML
  XGBoost
  Isolation Forest
  Prophet
  APIs
  OpenWeatherMap
  OpenAQ
  NewsAPI

Status
  Phase 1 — Ideation
  Problem validated
  System designed
  Prototype pending

Team
  Bannari Amman Institute of Technology, Erode
    Anusha S — Full Stack
    Abinaya S — Backend & ML
    Jeyashri M — UI/UX
    Kamalikaa K — Data

Final Thought
Friday morning.
School fees paid.
Family okay.
That’s not a feature.
That’s the goal.

RiderNet
Because no rider should lose income to the weather.

