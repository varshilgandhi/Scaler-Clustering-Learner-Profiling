# Scaler – Learner Profiling with Manual and Unsupervised Clustering

This project involves segmenting learners from Scaler based on company, job role, and experience using both manual and unsupervised clustering techniques. The goal is to identify standout profiles, high-performing clusters, and provide insights into salary trends across roles and companies.

---

## 📊 Problem Statement

Scaler wants to understand the profile of top-performing professionals in its network. Using anonymized data on company, job position, and compensation, this project clusters learners to identify meaningful patterns and help Scaler recommend better career paths and compensation benchmarks.

---

## 📁 Dataset Overview

The dataset contains:
- `Email_hash` – anonymized individual identifier
- `Company_hash` – anonymized current employer
- `orgyear`, `CTC`, `Job_position`, `CTC_updated_year`
- Derived fields like `Years of Experience`

---

## 🛠️ Tools & Concepts Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Regex, LabelEncoder, StandardScaler
- K-Means Clustering, Hierarchical Clustering
- Manual Flag-Based Clustering

---

## 📈 Project Workflow

1. **Data Cleaning & EDA**
   - Removed duplicates, cleaned company names using regex
   - Created new features like `Years of Experience`
2. **Manual Clustering**
   - Created 3 flags: `Designation`, `Class`, and `Tier` using CTC comparisons
   - Analyzed high/low performers by company, department, and experience
3. **Unsupervised Clustering**
   - Checked clustering tendency (Hopkins score)
   - Used Elbow method to determine optimal K
   - Applied K-Means and Hierarchical clustering
   - Visualized clusters and identified profiles
4. **Insights**
   - Top 10 companies by average CTC
   - Best paying roles by department and experience
   - Detected high-earning and underpaid segments

---

## 📌 Key Insights

- Tier 1 learners were mostly clustered in top-paying companies with 6–8 years of experience.
- Class 1 professionals in data science outperformed peers within the same companies.
- Clear stratification of compensation was observed between companies and roles.
- K-means validated the effectiveness of manual clustering structure.

---

## 💡 Business Recommendations

- Use manual cluster flags to power personalized recommendations to learners.
- Target partnerships with Tier 1 companies hiring high-CTC roles.
- Help learners in Tier 3 or Class 3 move to better roles or companies via upskilling.
- Use cluster insights to fine-tune Scaler’s placement support and pricing models.

---

## 📂 Files Included

- `Scaler_Clustering_Analysis.ipynb` – Main notebook
- `scaler_kmeans.csv` – Dataset
- `README.md` – This file
- (Optional) Cluster visuals or HTML export

---

## 🤝 Let’s Connect

Open to feedback and collaboration! [LinkedIn](https://www.linkedin.com/in/varshil-gandhi-08470b200/)
