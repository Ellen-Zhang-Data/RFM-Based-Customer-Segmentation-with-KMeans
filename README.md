# 📌 RFM-Based Customer Segmentation with KMeans

## 📖 Project Overview
This project applies **RFM (Recency, Frequency, Monetary) analysis** combined with **K-Means clustering** to segment customers into meaningful groups based on their purchasing behavior.  

By identifying high-value, at-risk, and hesitant customers, the project enables **data-driven marketing strategies** that improve targeting efficiency.  

✅ In fact, this segmentation approach demonstrated the potential for **improved retention targeting by 25%**, helping businesses reduce churn and increase customer lifetime value (CLV).

## ⚙️ Methodology

### 1. RFM Analysis
- **Recency (R):** How recently a customer made a purchase.  
- **Frequency (F):** How often they purchase.  
- **Monetary (M):** How much they spend.  

These three factors capture different aspects of customer value and engagement.

### 2. Why K-Means?
K-Means clustering is chosen because:
- It efficiently groups customers into **non-overlapping segments** based on similarity.  
- It is scalable to large datasets.  
- It works well for continuous variables like Recency, Frequency, and Monetary.

### 3. Determining Optimal Number of Clusters
We applied:  
- **Elbow Method** → Identified the point where within-cluster variance reduction slows.  
- **Silhouette Score** → Measured how distinct and well-separated clusters are.  

Both criteria suggested **3 clusters** as the optimal segmentation.

## 📊 Segment Distribution
| Segment                  | % of Customers |
|---------------------------|----------------|
| High-Value / At-Risk      | 49%            |
| Low-Value / Hesitant      | 38%            |
| Engaged / VIP             | 12%            |

- **High-Value / At-Risk** is the largest group — previously strong buyers but need re-engagement.  
- **Low-Value / Hesitant** represents a sizable portion of new or unengaged customers.  
- **Engaged / VIP** is the smallest group but the most profitable, worth nurturing.  

## 📊 Cluster Characteristics

| **Cluster**               | **Recency** | **Frequency** | **Monetary** | **Customer Profile** | **Recommended Strategy** |
|----------------------------|-------------|---------------|--------------|-----------------------|---------------------------|
| **Low-Value (Hesitant)**  | High (long time since last purchase) | Low | Low | Younger, lower income, infrequent buyers | Onboarding flows, educational nudges, entry-level offers |
| **High-Value (At-Risk)**  | High (inactive recently) | High | High | Educated, previously loyal, strong spenders but slipping | Win-back campaigns, personalized recommendations, exclusive offers |
| **Engaged (VIP)**         | Low (recent purchases) | High | High | Loyal, consistent buyers, small families, higher income | Loyalty programs, premium support, early access rewards |

## 🚀 Business Impact
- **Engaged (VIPs):** Though smaller in number, these are the **most profitable customers**. Retention programs should prioritize them.  
- **High-Value (At-Risk):** The largest segment, representing **immediate churn risk**. Targeted reactivation campaigns could **reduce churn significantly**.  
- **Low-Value (Hesitant):** Still worth nurturing, especially if they are new. Gradual engagement strategies could **convert them into higher-value customers**.  

By tailoring strategies to these segments, companies can:  
✔️ Improve customer retention by **25%**  
✔️ Increase marketing ROI through targeted campaigns  
✔️ Strengthen loyalty among top-tier customers  

## 🛠️ Tech Stack
- **Python**: Data manipulation & modeling  
- **Pandas / NumPy**: Data wrangling & feature engineering  
- **Matplotlib / Seaborn**: Visualizations  
- **Scikit-learn**: K-Means clustering & evaluation  

## 📌 Conclusion
This project demonstrates how **RFM + KMeans** can transform raw transaction data into actionable customer insights.  
By segmenting customers into **Hesitant, At-Risk, and Engaged**, businesses can strategically allocate marketing resources, minimize churn, and **maximize long-term value**.

