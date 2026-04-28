# AIinDrive
# AgroScoring — AI-driven Subsidy Distribution System

This project was developed during the **Decentrathon 5.0 Hackathon** for the **AI for Government (inDrive & Government of Kazakhstan)** track.

## 📌 Project Overview

AgroScoring is an intelligent scoring system designed to automate and bring transparency to the process of distributing agricultural subsidies in Kazakhstan. The current manual process of subsidy allocation often leads to regulatory overload, inefficient resource distribution, and "first-come, first-served" biases.

Our solution implements a data-driven approach to evaluate livestock farmers based on their infrastructure, production dynamics, and compliance with state regulations (based on the "Rules for subsidizing livestock development").

## 👥 Team & Roles

* **ML Developer:** [Nazar](https://github.com/eclipsen8) — Developed the scoring logic, predictive models, and explainability module.
* **Frontend Developer:** [Aruzhan](https://github.com/arrushhhh) — Created the "Smart Farmer's Cabinet" UI and interactive scoring dashboard.
* **Backend Developer:** [Abdanur](https://github.com/MnstrsParago) — (Backend was planned but not fully implemented for this prototype).

## 🚀 Key Features

* **Smart Scoring Engine:** Evaluates applications based on multiple criteria:
    * **Infrastructure:** Milking equipment, water supply, and certifications.
    * **Production Dynamics:** Growth in production efficiency (e.g., milk yield, livestock growth).
    * **Regulatory Norms:** Compliance with sanitary and technical standards.
    * **Land Sufficiency:** Analysis of pasture and forage availability.
* **AI Explainability (SHAP):** Every decision is backed by a clear explanation, showing the farmer exactly which factors influenced their final score.
* **Interactive Farmer Cabinet:** A user-friendly dashboard for farmers to input data and receive instant preliminary scoring results.

## 🛠 Technical Stack

### Machine Learning (ML)
* **Language:** Python
* **Model:** LightGBM (Gradient Boosting) for high-accuracy classification and scoring.
* **Interpretability:** SHAP (SHapley Additive exPlanations) to provide transparency for the government and farmers.
* **Data Processing:** Pandas, NumPy, Scikit-learn.

### Frontend
* **Technologies:** HTML5, CSS3 (Custom design system), JavaScript (Vanilla).
* **UX/UI:** Focused on high readability and interactive data visualization for rural users.

## 📊 ML Logic Details

The ML model processes historical and real-time data to predict the eligibility and efficiency of a subsidy request. 
- **Preprocessing:** Label Encoding for categorical features and rigorous cleaning of regulatory data.
- **Thresholding:** The system uses a calibrated threshold (e.g., 20/100 points) to filter out high-risk applications while providing constructive feedback to those who fall short.
- **Metrics:** Evaluated using ROC-AUC and Accuracy to ensure fairness in decision-making.

## ⚠️ Current Status

The project is currently a **functional prototype (Frontend + ML Logic)**. 
- The ML model is trained and tested in a Jupyter Notebook environment.
- The Frontend is a static interactive prototype demonstrating the user journey.
- **Note:** Due to time constraints during the hackathon, the backend integration and API development were not completed.

## 📜 Acknowledgments

Developed as part of **Decentrathon 5.0** to address real-world governance challenges in the Republic of Kazakhstan through the power of Artificial Intelligence.
