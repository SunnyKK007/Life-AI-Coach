# 🧬 LifeAI Health Coach
> **A unified, edge-AI-powered digital health ecosystem utilizing real-time localized machine learning to eliminate fragmented health tracking.**
![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
## 📌 Overview
Modern digital health relies on isolated systems (separate apps for nutrition, activity, and medical monitoring). LifeAI solves this "data silo bottleneck" by acting as a centralized intelligence engine. 
By leveraging **React Native's New Architecture (JSI)** and **Edge Machine Learning**, LifeAI processes user health data synchronously on the device GPU—ensuring zero latency, absolute privacy, and proactive health interventions.
## 🧠 The Edge Data Pipeline
LifeAI utilizes local inference to process physiological data instantly without cloud dependency.
`[Mobile Camera] ➔ [TF.js Edge CV] ➔ [JSI Telemetry Sync] ➔ [ExecuTorch LLM] ➔ [Contextual AI Output]`
## 🏗️ Technical Architecture
### Polyglot Database Design
To handle disparate data types efficiently, the backend utilizes a multi-database architecture:
*   **PostgreSQL (Relational):** Secure user authentication, profile biometrics, and structured food logs.
*   **MongoDB (Time-Series):** High-throughput ingestion of background wearable telemetry (steps, sleep).
*   **ChromaDB / pgvector (Vector):** Semantic embeddings for the local RAG pipeline to power the AI coach.
### Tech Stack

| Domain | Technologies |
| :--- | :--- |
| **Mobile Core** | React Native (TypeScript), New Architecture (JSI / Fabric) |
| **Edge AI (JS Inference)** | TensorFlow.js (WebGL), `react-native-executorch`, Hugging Face Quantized LLMs |
| **Backend API** | FastAPI (Python 3.11+), Uvicorn, WebSockets |
| **Telemetry Sync** | Apple HealthKit (iOS), Google Health Connect (Android) |

## 🚀 Features & Phased Rollout
### Phase 1: Core Consumer MVP (Current)
*   **AI Health Coach:** 24/7 hyper-personalized conversational agent running entirely on-device via a local RAG architecture.
*   **CV Food Scanner:** Real-time volumetric and macronutrient estimation directly from the camera viewfinder via TensorFlow.js.
*   **Wearable Syncing:** Silent, battery-efficient background syncing of step counts and sleep cycles via native OS APIs.
*   **Human Safety Net:** A React-based B2B operational dashboard for clinicians to monitor flagged anomalies via WebSockets.
### Phase 2: Medical & Enterprise Scale (Upcoming)
*   **Clinical Hardware Sync:** Direct BLE integrations for Dexcom/Abbott CGMs and Omron blood pressure cuffs.
*   **Predictive ML Risk Engine:** XGBoost classification models utilizing behavioral metadata to forecast user churn and metabolic regressions.
*   **Enterprise B2B Portals:** Anonymized population health analytics for corporate HR departments.
## 💻 Getting Started (Local Development)
Because this is a React Native project, a single JavaScript codebase deploys to both iOS and Android natively.
### Prerequisites
*   [Node.js](https://nodejs.org/) (v18+)
*   [Android Studio](https://developer.android.com/studio) (for Android SDKs and Emulator)
*   [Xcode](https://developer.apple.com/xcode/) (Mac only, for iOS Simulator and CocoaPods)
### Installation
1. Clone the repository:
```bash
   git clone [https://github.com/yourusername/LifeAI-Health-Coach.git](https://github.com/yourusername/LifeAI-Health-Coach.git)
   cd LifeAI-Health-Coach
