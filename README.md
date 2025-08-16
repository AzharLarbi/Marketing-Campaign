# Data driven Customer Targeting Campaign Optimization

## Project Overview
This project applies machine learning to predict customer responses to a marketing campaign, with the goal of helping businesses **improve targeting, reduce wasted spend, and increase campaign ROI**.  

We analyze customer demographics, prior campaign interactions, and spending habits to build predictive models using logistic regression, decision trees, and random forests. The outcome is a framework that not only forecasts campaign responses, but also highlights which customer attributes drive engagement.

---

## Problem Statement
Marketing campaigns can be costly, and ineffective targeting often leads to wasted resources. By predicting which customers are most likely to respond, businesses can:  

- Focus campaigns on high-probability responders.  
- Personalize offers for different customer segments.  
- Reduce acquisition costs while increasing conversion rates.  

This project addresses the following questions:  
- Which customer attributes most strongly influence campaign response?  
- How accurately can machine learning models forecast campaign outcomes?  
- What actionable insights can marketers derive to improve campaign efficiency?  

---

## Data Description
Dataset source: [Kaggle Marketing Campaign Dataset](https://www.kaggle.com/datasets/rodsaldanha/arketing-campaign)  

The dataset includes customer and campaign data such as:  
- **Customer Demographics:** Income, marital status, education, household composition.  
- **Campaign Interactions:** Previous campaign responses, current campaign response (target), days since last purchase, complaints.  
- **Spending Behavior:** Purchases across product categories (e.g., wines, meat, sweets).  
- **Target Variable:** `Response` (1 = accepted campaign offer, 0 = did not accept).  

---

## Exploratory Data Analysis (EDA)
Key insights from EDA included:  
- **Income:** Higher income customers were more likely to respond.  
- **Campaign History:** Past responders were more likely to engage again.  
- **Complaints:** Customers with prior complaints were less likely to respond.  
- **Education:** Graduate and Ph.D. holders showed higher response rates.  


---

## Business Insights
From the analysis, several actionable takeaways emerged:  

1. **Income as a Predictor of Engagement**  
   - Higher-income customers are more likely to respond.  
   - Campaigns can be optimized by allocating more resources to this segment.  

2. **Leverage Past Responders**  
   - Customers who accepted past campaigns are strong candidates for re-engagement.  
   - Building loyalty programs around this group could increase long-term ROI.  

3. **Customer Complaints Hurt Response Rates**  
   - Dissatisfied customers are less likely to respond.  
   - Improving customer service may indirectly improve campaign effectiveness.  

4. **Education Matters**  
   - Higher-educated customers respond at greater rates.  
   - Campaigns can be tailored with messaging or offers that resonate with this demographic.  

5. **Timing & Frequency Influence Success**  
   - Customers who purchased recently are more likely to respond.  
   - Aligning campaigns with recent interactions can lift conversion rates.  

---

## Future Directions
- Explore advanced models such as gradient boosting or ensemble stacking.  
- Engineer interaction features (e.g., combining spending and recency).  
- Develop a deployment pipeline for real-time campaign scoring.  
- Create dashboards for marketers to visualize customer segments and predicted response rates.  

---

## Usage
1. Load and preprocess the dataset.  
2. Run EDA to understand key drivers.  
3. Train logistic regression, decision tree, and random forest models.  
4. Evaluate models with accuracy and feature importance metrics.  
5. Apply insights to design more effective, targeted campaigns.  
