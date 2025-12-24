# 📊 Churn Prediction with Modern A/B Testing

## 🔎 Overview
This project explores customer churn prediction using machine learning and modern experimentation techniques.  
It combines **Exploratory Data Analysis (EDA)**, **predictive modeling**, and **advanced A/B testing simulations** (classic, personalized, and multi-armed bandits) to deliver actionable business insights.

Developed an end‑to‑end churn prediction pipeline combining EDA, machine learning (Logistic Regression, Random Forest, XGBoost), and experimentation (A/B testing, multi‑armed bandits). Achieved ROC‑AUC of 0.91 and identified mid‑tenure customers as highest churn risk (81% in Very High tier). Demonstrated that adaptive bandit strategies converge on the most effective retention offer, reducing churn by ~27%.

---

## 📂 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed customer features (Years, Account_Manager, Total_Purchase, Num_Sites, etc.).
- Key insights:
  - Churn risk increases sharply after **5 years of tenure**, peaking at **81% in Very High risk tier**.
  - Customers with account managers churned more (19.4% vs 14.1%), suggesting reactive engagement.

### 2. Modeling
- Compared **Logistic Regression, Random Forest, and XGBoost**.
- **Logistic Regression** achieved the best balance:
  - ROC-AUC: **0.91**
  - Recall: **0.73**
- Random Forest delivered high precision but low recall.
- XGBoost underperformed on this dataset.

### 3. Customer Scoring & Segmentation
- Converted model outputs into churn probabilities.
- Segmented customers into **Low, Medium, High, Very High risk tiers**:
  - Low risk: 3% churn
  - Medium risk: 20% churn
  - High risk: 29% churn
  - Very High risk: 81% churn

### 4. Modern A/B Testing
- **Classic A/B Test:** blanket retention offers reduced churn modestly.
- **Personalized A/B Test:** targeting Medium/High/Very High risk customers improved efficiency.
- **Multi-Armed Bandit Simulation:** adaptively learned that *Premium Support* was the most effective retention strategy (~27% uplift).

---

## 📊 Results
- Identified **mid-tenure customers (5–7 years)** as highest churn risk.
- Account manager program requires redesign.
- Logistic Regression is the most effective model for churn prediction.
- Adaptive bandit strategies converge on the best retention offer, saving costs and maximizing retention.

---

## 🚀 Tech Stack
- **Python** (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn)
- **Machine Learning**: Logistic Regression, Random Forest, XGBoost
- **Experimentation**: Classic A/B Testing, Personalized A/B Testing, Multi-Armed Bandits

---

## 📌 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/churn-prediction-ab-testing.git
