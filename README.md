# 🧬 LifeAI Health Coach
> **A unified, edge-AI-powered digital health ecosystem utilizing real-time localized machine learning to eliminate fragmented health tracking.**
![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
## 📌 The Problem: The Data Silo Bottleneck
Modern digital health relies on isolated systems—users track nutrition in one app, steps in another, and medical vitals in a third. 
1. **Context Disconnect:** A glucose spike lacks the context of the user's logged carbohydrates.
2. **Cognitive Friction:** Manual logging across multiple apps drives high user churn.
3. **Reactive Systems:** Existing apps act as historical ledgers rather than proactive, predictive agents.
## 🧠 The Solution: Edge Intelligence Flow
LifeAI acts as a centralized intelligence engine. By leveraging **React Native's New Architecture (JSI)**, the app processes physiological data synchronously on the device GPU—ensuring zero latency, absolute privacy, and proactive interventions.
`[Mobile Camera] ➔ [TF.js Edge CV] ➔ [JSI Telemetry Sync] ➔ [ExecuTorch LLM] ➔ [Contextual AI Output]`
## 🏗️ Technical Architecture
### 1. Polyglot Database Design
To handle disparate data types efficiently, the Python backend utilizes a multi-database architecture:
*   **PostgreSQL (Relational):** Secure user authentication, profile biometrics, and structured food logs.
*   **MongoDB (Time-Series):** High-throughput asynchronous ingestion of background wearable telemetry.
*   **ChromaDB / pgvector (Vector):** Semantic embeddings for the local RAG pipeline to power the AI coach.
### 2. Core Tech Stack

| Domain | Technologies |
| :--- | :--- |
| **Mobile Core** | React Native (TypeScript), New Architecture (JSI / Fabric) |
| **Edge AI (JS Inference)** | TensorFlow.js (WebGL), `react-native-executorch`, Hugging Face Quantized LLMs |
| **Backend API** | FastAPI (Python 3.11+), Uvicorn, WebSockets |
| **Telemetry Sync** | Apple HealthKit (iOS), Google Health Connect (Android) |

## 🚀 Execution Roadmap
### Phase 1: Core Consumer MVP (Current)
*   **AI Health Coach:** 24/7 hyper-personalized conversational agent running entirely on-device via a local RAG architecture.
*   **CV Food Scanner:** Real-time volumetric and macronutrient estimation directly from the camera viewfinder via TensorFlow.js.
*   **Wearable Syncing:** Silent, battery-efficient background syncing of step counts and sleep cycles via native OS APIs.
*   **Human Safety Net:** A React-based B2B operational dashboard for clinicians to monitor flagged anomalies via WebSockets.
### Phase 2: Medical, Predictive & Enterprise Expansion (Upcoming)
*   **Clinical Hardware Sync:** Direct BLE integrations for Dexcom/Abbott CGMs and Omron blood pressure cuffs.
*   **Predictive ML Risk Engine:** Custom XGBoost classification models utilizing behavioral metadata to proactively forecast user churn and metabolic regressions.
*   **Enterprise B2B Portals:** Anonymized population health analytics and community step-challenges for corporate HR departments.
## 💻 Local Development Setup
Because this is a React Native project, a single TypeScript codebase deploys to both iOS and Android natively. 
### Prerequisites
*   **Node.js (v18+):** Required to run the Metro Bundler (the local development server that compiles JavaScript) and manage `npm` packages. *(Note: The backend API runs independently on Python/FastAPI).*
*   **Android Studio:** Provides the Android SDK and AVD Emulator for local Android testing.
*   **Xcode (Mac only):** Provides the iOS Simulator and CocoaPods for linking native iOS libraries.
### Installation
1. Clone the repository and install the JavaScript dependencies:
```bash
   git clone [https://github.com/yourusername/LifeAI-Health-Coach.git](https://github.com/yourusername/LifeAI-Health-Coach.git)
   cd LifeAI-Health-Coach
   npm install
