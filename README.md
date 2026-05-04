# 📊 TikTok Claim vs Opinion Classification

## 📌 Project Overview
This project builds machine learning models to classify TikTok videos as:

- **Claim (1)**
- **Opinion (0)**

The objective is to support content moderation by automatically identifying potentially misleading or high-risk content.

---

## 🎯 Objectives
- Perform Exploratory Data Analysis (EDA)
- Engineer meaningful features
- Train multiple ML models
- Compare model performance
- Select the best model

---

## 📂 Dataset
The dataset includes:

- `video_view_count`
- `video_like_count`
- `video_comment_count`
- `video_share_count`
- `video_duration_sec`
- `author_ban_status`
- `claim_status` (target)

---

## 🔍 Key Insights

- Claim videos receive **higher engagement**
- Suspicious/banned accounts post more claims
- Engagement metrics strongly influence classification
- Video duration has little impact

---

## 🛠️ Feature Engineering

Created normalized engagement features:

- `likes_per_view`
- `comments_per_view`
- `shares_per_view`

---

## 🤖 Models Used

- Logistic Regression
- Random Forest
- XGBoost ✅

---

## 📊 Model Performance Comparison

| Model                | Accuracy | Precision | F1 Score | 
|---------------------|----------|----------|--------|
| Logistic Regression | 62%      | 58%      | 70%    | 
| Random Forest 🚀    | 99.6%    | 100%     | 99.6%    | 
| XGBoost           | 99.3%   | 99.8%     | 99.3%    | 

---

## 🏆 Best Model

**Random Forest performed best** with:

- Highest accuracy
- Strong precision & recall balance
- Minimal false negatives (critical for detecting claims)

---

## 📦 Confusion Matrix Insight

- **False Positive (FP):** Opinion predicted as Claim  
- **False Negative (FN):** Claim predicted as Opinion  

⚠️ Minimizing **False Negatives** is most important because:
Missing a claim can allow harmful content to spread.

---

## 🚀 Business Impact

This model helps:

- Prioritize moderation queue
- Reduce manual workload
- Detect risky content faster
- Improve platform safety

---

## 🧰 Tools & Technologies

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- XGBoost

---

## 📁 Project Structure
- ├── README.md
- ├── tiktok_claim_analysis.ipynb
---

## 🏁 Conclusion

This project demonstrates how machine learning can effectively classify social media content using engagement patterns and behavioral signals.

---

## 👤 Author

**MD. SAIFUL ISLAM**  
Aspiring Data Analyst | Google Advanced Data Analytics Certificate
