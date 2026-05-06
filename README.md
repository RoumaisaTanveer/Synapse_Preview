# Synapse — AI-Powered Team Matching Platform Preview

_**Connect minds, Build teams**_

---

## 📌 What is Synapse?

Synapse is an intelligent team formation platform built for student developers and project collaborators. It goes beyond basic skill matching by combining:

- Heuristic scoring  
- Personality clustering  
- Machine learning  

This ensures teams are not just technically compatible — but also **interpersonally effective**.

---

## 🚀 Key Features

- **3-Layer Hybrid Matching Engine**  
  Skill coverage + personality clustering + ML-based prediction  

- **SHAP Explainability**  
  Every match includes a clear explanation  

- **Proximity-Aware Matching**  
  GPS-based cohort filtering  

- **Volunteer Mentor System**  
  Special matching logic for mentors  

- **Real-Time Messaging**  
  Auto-created group chats on team confirmation  

- **Project Health Dashboard**  
  Tracks conflict safety, velocity, and engagement  

- **React Admin Panel**  
  Live analytics with API integration  

---

## 🛠 Tech Stack

| Layer            | Technology |
|-----------------|-----------|
| Backend         | FastAPI, Python 3.12 |
| Database        | PostgreSQL (JSONB, pgAdmin) |
| Mobile Client   | Flutter |
| Admin Panel     | React |
| ML Engine       | scikit-learn (K-Means, Random Forest), SHAP |
| Auth            | JWT |
| Notifications   | Firebase FCM |
| Deployment      | Uvicorn + Procfile |

---

## 🧠 Matching Algorithm

Synapse uses a **3-layer weighted hybrid approach**:
Final Score = 0.60 × Heuristic + 0.20 × Personality + 0.20 × ML Predictor

### 🔹 Layer 1 — Heuristic Skill Coverage (60%)
- Uses a `min()` cap formula across 33 skill domains  
- Prevents over-reliance on a single shared skill  

### 🔹 Layer 2 — Personality Clustering (20%)
- K-Means clustering on Big Five (OCEAN) + DISC traits  
- 6 clusters  
- Prefers complementary personalities over identical ones  

### 🔹 Layer 3 — Random Forest Predictor (20%)
- Trained on historical team performance data  
- SHAP values explain match decisions  

### ⚡ Soft Factors (Overlayed)
- Mood score  
- Cohort proximity (Haversine distance)  
- Role diversity bonus  
- Budget alignment  

---

## 📂 Project Structure
## 📂 Project Structure

    app/
    ├── api/v1/
    │   ├── auth.py
    │   ├── matching.py
    │   ├── profiles.py
    │   ├── teams.py
    │   ├── messaging.py
    │   ├── mentors.py
    │   ├── project_health.py
    │   ├── project_tasks.py
    │   ├── admin.py
    │   ├── feedback.py
    │   └── roles.py
    │
    ├── core/
    │   ├── team_builder.py
    │   ├── mentor_matching.py
    │   ├── profile_scorer.py
    │   ├── feedback_engine.py
    │   ├── messaging_engine.py
    │   ├── checkin_service.py
    │   ├── security.py
    │   └── config.py
    │
    ├── models/      # SQLAlchemy models
    ├── schemas/     # Pydantic schemas
    ├── services/    # Email & push notifications
    └── db/          # Database session

    suggestive_matching_engine/
    ├── algorithms/
    │   ├── matching.py
    │   ├── clustering.py
    │   └── predictor.py
    └── app.py

---

## 🔗 Key API Endpoint


GET /matching/suggestions?top_n=5&task_type=backend&explain=true


Returns ranked team suggestions with **SHAP-based explanations**.

---

## 📊 Project Status

 **Final Year Project at PUCIT**  


---

## 🎥 Demo

- 🔗 Coming Soon  
- 📄 FYP Report / Research Paper — available on request  

---

## 📎 Notes

This repository is intended for **public showcase** and demonstration purposes.

---
## 🔒 Repository Scope

This repository is intended for **demonstration and showcase purposes only**.

Core components such as the **matching engine, proprietary algorithms, and production-level logic are not included** in this public version.

If you are interested in the full system design or implementation details, feel free to reach out.
