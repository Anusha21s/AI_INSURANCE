🎯 Phase 2 Goal

“Protect Your Worker”

In this phase, RiderNet evolves from concept to a functional prototype that demonstrates:

✅ Rider onboarding
✅ Weekly policy creation
✅ Dynamic premium calculation
✅ Automated claim triggering
✅ Smart claim validation & payout decision
👤 Target Persona

Focused Persona: Full-Time Food Delivery Rider (e.g., Swiggy / Zomato)

Example:
Karthik — depends fully on daily delivery income and is highly affected by weather disruptions.

🧩 Core Features Implemented
1️⃣ Registration Process ✅
Mobile number / basic details onboarding
GPS-based location capture
Device fingerprinting initialized
Rider categorization:
Full-time
Part-time
Rural

👉 Output: Rider profile created with a baseline risk score

2️⃣ Insurance Policy Management ✅
Weekly subscription model implemented

Plans:

Basic — ₹29
Standard — ₹49
Premium — ₹79

👉 Features:

Activate / deactivate policy
View active coverage
Weekly renewal simulation
3️⃣ Dynamic Premium Calculation (AI-Based) ✅

We implemented a rule-based + ML-ready hybrid model.

Inputs:

Weather risk (rain, heat, AQI)
Location risk (flood-prone zones)
Rider activity history
Fraud risk score

Output:

Dynamic weekly premium

Example Calculation:

Base = ₹29  
+ Rain Risk = ₹10  
+ Location Risk = ₹5  
- Safe Zone Discount = ₹2  

Final Premium = ₹42/week

👉 ML-ready architecture using XGBoost (planned integration)

4️⃣ Claims Management (Zero-Touch System) ✅

Automated Claim Flow:

Event detected (via API/mock)
System validates:
Rider location
Activity status
Policy validity
Claim automatically created
Fraud checks applied
Decision generated:
✅ Approved → payout triggered
⚠️ Suspicious → flagged
🌦️ Parametric Triggers Implemented
Trigger	      Condition	           Payout
🌧 Rain     	> 60 mm	              100%
🔥 Heat	     > 45°C	               50%
🌫 AQI	      > 400	                Partial
🚫 Bandh	     Verified (mock API)	 100%

👉 APIs Used:

OpenWeatherMap (weather data)
OpenAQ (air quality)
NewsAPI (bandh detection — mock logic)
🛡️ Fraud Detection (Phase 2 - Basic)

(Advanced system will be implemented in Phase 3)

Implemented Checks:

GPS consistency validation
No teleportation (>5 km jump detection)
Rider activity validation (must be active)
New user payout cap (50%)

👉 Output:

Risk score generated
Claim allowed or flagged
⚙️ System Architecture
Frontend (React + Vite)
        ↓
API Layer (FastAPI)
        ↓
Services:
  - Auth Service
  - Policy Engine
  - Claim Engine
  - Risk Engine
        ↓
Database (PostgreSQL)
        ↓
External APIs:
  - Weather
  - AQI
  - News (mock)
🔄 Workflow (End-to-End)
Rider registers
Selects weekly plan
Premium calculated dynamically
System monitors environment
Disruption detected (e.g., heavy rain)
Claim auto-triggered
Fraud checks executed
Payout decision generated
📊 Demo Scenario

Scenario: Heavy Rain Day

Rider: Karthik (Active)
Rain > 65 mm detected
System triggers claim automatically
Fraud check passed
₹750 payout approved instantly
📱 UI Features (Prototype)
Simple onboarding (2 minutes)
Dashboard:
Active policy
Earnings protected
Real-time alerts:
“Heavy rain detected — claim initiated”
Multi-language support (planned)
💻 Tech Stack
Frontend
React
Vite
TailwindCSS
Backend
FastAPI
PostgreSQL
AI/ML (Phase 2 Level)
Rule-based system
ML-ready pipeline
XGBoost (planned)
APIs
OpenWeatherMap
OpenAQ
NewsAPI (mock integration)
📦 Repository Structure
RiderNet/
│
├── frontend/
├── backend/
│   ├── routes/
│   ├── services/
│   ├── models/
│   └── utils/
│
├── ml-models/
├── docs/
└── README.md

💡 Final Thought

RiderNet is no longer just an idea — it is a working income protection system.

🛵 Because no rider should lose income to the weather.
