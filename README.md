# Smart Squad AI: FIFA Tactical AI (Virtual Coach) ⚽🤖

[![Award - IEEE Winner](https://img.shields.io/badge/IEEE%20Project%20Exhibition-Winner%20%F0%9F%8C%9F-cyan?style=for-the-badge)](https://www.linkedin.com/in/saim-awan-530730269/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)](https://python.org)
[![Framework](https://img.shields.io/badge/Machine%20Learning-Ensemble-ff007f?style=for-the-badge)](https://scikit-learn.org)

**Smart Squad AI** is a comprehensive, end-to-end data science pipeline and machine learning application designed for grassroots and semi-professional football coaching staff. The system eliminates subjective observer bias by mapping a 7-dimensional technical/physical player attribute space to optimal tactical roles on the pitch using a heterogeneous soft-voting ensemble.

> 🏆 **Award-Winning Project:** Awarded **1st Place / Shield Winners** at the Bahria University Project Exhibition by an evaluation panel of IEEE Seniors.
<img width="900" height="1200" alt="WhatsApp Image 2026-05-21 at 10 33 13 PM" src="https://github.com/user-attachments/assets/4461e0cb-08c2-42f0-ae60-2974a3e800a0" />
<img width="960" height="1280" alt="WhatsApp Image 2026-05-21 at 10 33 09 PM" src="https://github.com/user-attachments/assets/849172ed-ce7c-44bb-b317-db1f860093e0" />

---

## 🧭 Core Features & Coaching Value

* **Predictive Role Assignment Engine:** Inputs individual player profiles via custom sliders and outputs multi-class position probabilities.
* **Algorithmic Scouting Matrix:** Computes vector proximity using NumPy Euclidean distance over a 27,000-record historical database to discover the Top 3 real-world professional alternative profiles.
* **Dynamic Radar Overlays:** Renders real-time visual attribute comparisons using inline Matplotlib canvases.
* **Tactical Board Optimization:** Auto-populates complex formation slots (4-3-3, 4-4-2, 3-5-2, 5-4-1, 4-2-3-1) with the highest-probability squad assets using custom assignment fallbacks.
* **Deterministic Set-Piece Rationale:** Calculates optimal corner, free-kick, and penalty takers using custom-weighted domain attribute formulas.

---

## 📊 The Machine Learning Architecture

To optimize the **Bias-Variance Tradeoff**, the core engine implements a **Heterogeneous Soft Voting Classifier** combining five diverse statistical learning paradigms:

1.  **Support Vector Machine (SVM):** Maximizes linear hyperplane separation boundaries using standard scaled spaces.
2.  **Logistic Regression (LR):** Establishes parametric baselines with well-calibrated position confidence probabilities.
3.  **Random Forest (RF):** Reduces variance (Bagging) through depth-constrained (`max_depth=8`) parallel estimators.
4.  **Gradient Boosting (GB):** Reduces bias (Boosting) sequentially by fitting estimators to residual classification errors.
5.  **K-Nearest Neighbors (KNN):** Evaluates non-parametric spatial clusters to anchor target classifications and scouting similarity calculations.

---

## 🛠️ Data Science Pipeline Workflow

1.  **Ingestion:** Concat chunks across historical public SoFIFA telemetry datasets (~54,000 records raw capped at 27,000 stratified instances).
2.  **Cleaning:** Mitigates target label noise by executing string-splitting on multi-label strings to isolate primary target vectors. Imputes domain-specific structural default weights ($Goalkeeping=10$).
3.  **Transformation:** Fits a global `StandardScaler` (Z-score normalization) for gradient and boundary optimization while preserving unscaled metrics for vector distance queries.
4.  **Deployment:** Persists the complete data product natively via a local Tkinter-driven UI running entirely offline.

---

## 🚀 Getting Started

### Prerequisites
* Python 3.8 or higher installed on your machine.

### Installation & Execution Steps



1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/megaop98/Smart-Squad-AI.git](https://github.com/megaop98/Smart-Squad-AI.git)
