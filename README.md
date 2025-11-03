# D-Project4: OpenRep Social Media Analytics Dashboard

This capstone project, in collaboration with **OpenRep**, focused on designing a full-stack **data pipeline and analytics dashboard** to evaluate social media engagement across multiple platforms — including Instagram, Twitter(X), LinkedIn, Pinterest, and Facebook.  
The system automated data ingestion, cleaning, anomaly detection, and visualization to support OpenRep’s content performance insights.

* **Dataset:** Multi-platform social media data (Instagram, X, Facebook, LinkedIn, Pinterest).  
* **Tools:** Python (Pandas, Plotly), R (ggplot2, dplyr), Tableau, Power BI.  
* **Techniques:** API data extraction, automated preprocessing, EDA, anomaly detection, KPI formulation, and dashboard visualization.  
* **Goal:** Create a centralized dashboard integrating platform-specific metrics to identify engagement trends and detect anomalies.

---

### ⚙️ Pipeline Overview

**1. API Development**
- Automated API converts platform data into structured Excel files.  
- Removed redundant columns, standardized field names, and validated schema consistency.  
- Generated seven cleaned datasets:
  - `fact_facebook`, `fact_instagram`, `fact_linkedin`, `fact_pinterest`, `fact_twitter`, `fact_gmb`, and `dim_post`.  

**2. Data Cleaning**
- Filled missing values using median imputation.  
- Dropped columns with >80% missing values.  
- Flagged residual errors for manual review.

**3. EDA**
- **Instagram:** Engagement, followers, impressions, and reach were strongly correlated.  
- **Twitter(X):** Clear anomaly clusters in July 2024 and January 2024; engagement spikes >850 followed by steep declines.  
- **Pinterest:** Lower but stable engagement patterns.  
- **Facebook:** High variance and isolated outlier peaks.  
- **LinkedIn:** Consistent moderate engagement rate and audience growth.

---

### 🔎 Post-Perspective Analytics

**KPI Formulas**
- *Engagement Rate* = Engagement ÷ Reach  
- *Like Rate* = Likes ÷ Reach  
- *Impressions per User* = Impressions ÷ Reach  

**Insights**
- Instagram and LinkedIn maintain consistent engagement and like rates.  
- Facebook occasionally yields top-performing viral posts.  
- Twitter(X) and Pinterest show wider metric dispersion, indicating platform volatility.  
- Facebook: strong re-exposure → brand recall;  
  Instagram + LinkedIn: balanced delivery;  
  Twitter + Pinterest: strong user acquisition but lower retention.

---

### 📊 Dashboard Framework

<div align="center">
  <img src="images/OP_Overview.png" alt="OpenRep Analytics Dashboard Overview" width="600"/>
</div>

- **Anomaly Detection:** Automatically flags metric spikes/drops (engagement, impressions, profile views).  
- **Custom Filters:** Users can select *platform* and *metric* (e.g., profile views, engagement rate, CTR, follower growth).  
- **Visualization Layers:**  
  - Platform-level engagement tracking  
  - Post-level performance analysis  
  - Cross-platform KPI comparisons  

<div align="center">
  <img src="images/OP_Instagram.png" width="450"/>
  <img src="images/OP_X.png" width="480"/>
</div>

<div align="center">
  <img src="images/OP_linkedin.png" width="450"/>
  <img src="images/OP_pinterest.png" width="450"/>
</div>

---

### 📈 Key Findings
- Instagram engagement rose steadily with clear seasonal anomalies (Mar 2024 & Mar 2025).  
- Twitter(X) recorded spikes in engagement and impressions but could not sustain post-peak activity.  
- LinkedIn maintained the most stable engagement rate across 2024–2025.  
- Post-level performance confirmed campaign-specific patterns (e.g., **Campaign-2819c4db-452c-43c3-8bec-267af48dcf41**).  

---

### 🧠 Skills Demonstrated
- Multi-platform API integration  
- Data cleaning and pipeline automation  
- Anomaly detection (EDA-driven)  
- KPI engineering and visualization design  
- Cross-team collaboration & presentation (MIT Sloan reference integration)  

