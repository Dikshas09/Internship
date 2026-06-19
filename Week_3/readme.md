# Week 3: AI Recommendation Logic (Tech Stack Recommender)

## 📌 Project Overview
This project marks the transition from passive data classification to **active prediction**. The goal is to build a content-based recommendation engine designed to tackle "choice overload" by acting as a digital matchmaker. Specifically, this application takes a user's raw technical skills and career goals and maps them mathematically to the most relevant job roles and toolsets.

---

## 🏗️ Architecture: The IPO Model
The system is built on a systematic **Input-Process-Output (IPO)** framework:

1. **Input (User State):** Ingests a minimum of three qualitative user skills/interests to ensure sufficient data density.
2. **Process (Similarity Logic):** 
   * Transforms raw text into numerical arrays using **TF-IDF (Term Frequency-Inverse Document Frequency)** weighting to reward highly specific terms and penalize generic words.
   * Calculates the geometric alignment between the user profile vector and job role vectors using **Cosine Similarity**.
3. **Output (Top-N List):** Truncates and sorts the results to display the **Top 3** highest-scoring, tailored career recommendations.

---

## 🛠️ Key Features & Methodologies

* **Content-Based Filtering:** Focuses entirely on item attributes (job role metadata from `raw_skills.csv`) rather than historical community behavior, making it immediately effective.
* **TF-IDF Weighting:** Moves past simple binary (1s and 0s) matching to understand the specific contextual importance of each skill.
* **Cosine Similarity:** Uses angular orientation ($cos(\theta)$) rather than Euclidean distance, making the recommendation metric invariant to the length or size of text descriptions.
* **Cold Start Bypass:** Mitigates user data scarcity by utilizing a targeted onboarding survey method (direct skill ingestion).

---

## 🚀 How to Run the Project

### Prerequisites
Make sure you have the required libraries installed:
```bash
pip install pandas numpy scikit-learn
