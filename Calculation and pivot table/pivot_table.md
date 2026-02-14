# Pivot Table Analysis

## Project  
User Engagement & Revenue Optimization Analysis for a Streaming Platform

---

## 1. Objective of Pivot Analysis

After cleaning and preparing the dataset, I created structured pivot tables to analyze:

- Revenue distribution across subscription tiers  
- User retention patterns  
- Engagement behavior across devices and content  
- Demographic consumption trends  
- Churn indicators  
- Monetization efficiency  

Each pivot table directly supports the core objective:

> Identifying key drivers of user engagement and revenue optimization.

---

## 2. Revenue by Subscription Plan

**Columns Used**
- subscription_plan  
- monthly_spend (SUM & AVERAGE)

**Purpose**  
To evaluate how different subscription tiers contribute to total revenue and spending behavior per user.

**Key Insights**
- PREMIUM generates the highest total revenue.  
- STANDARD shows the highest average spend per user.  
- BASIC contributes moderate revenue with lower ARPU.  

**Business Relevance**
- Identify high-performing pricing tiers  
- Design upgrade campaigns  
- Optimize pricing strategy  
- Focus marketing on high-value segments  

---

## 3. Active Rate (Retention Insights)

**Columns Used**
- subscription_plan  
- is_active (Count & % of Row)

**Purpose**  
To measure retention performance across subscription tiers.

**Key Insights**
- PREMIUM+ has the highest retention rate.  
- PREMIUM generates strong revenue but slightly lower retention.  
- Overall active rate ≈ 85%.  

**Business Relevance**
- Detect churn-prone segments  
- Design retention campaigns  
- Improve engagement in revenue-heavy tiers  

---

## 4. Engagement by Device Type

**Columns Used**
- device_type  
- watch_duration_minutes  
- progress_percentage  

**Purpose**  
To understand how device usage influences engagement.

**Key Insights**
- Tablet and Desktop users show higher watch duration.  
- Mobile users show slightly lower engagement time.  
- Completion rates are consistent across devices.  

**Business Relevance**
- Optimize mobile UX  
- Promote long-form content on larger screens  
- Build device-based personalization  

---

## 5. Revenue & Engagement by Country

**Columns Used**
- country  
- monthly_spend  
- watch_duration_minutes  
- count of is_active  

**Purpose**  
To evaluate geographic revenue concentration.

**Key Insights**
- USA contributes majority of revenue.  
- Engagement levels are similar in USA and Canada.  
- Revenue is geographically concentrated.  

**Business Relevance**
- Market expansion planning  
- Regional pricing evaluation  
- Reduce geographic dependency risk  

---

## 6. Engagement by Content Type

**Columns Used**
- content_type  
- watch_duration_minutes  
- imdb_rating  
- count of watch_date  

**Purpose**  
To evaluate content format performance.

**Key Insights**
- Documentaries & Limited Series show higher watch duration.  
- TV Series have slightly higher ratings.  
- Movies generate highest view volume.  

**Business Relevance**
- Balance content investment  
- Plan production strategy  
- Optimize content acquisition  

---

## 7. Genre vs Engagement

**Columns Used**
- genre_primary  
- progress_percentage  
- watch_duration_minutes  
- count of views  

**Purpose**  
To identify binge-worthy genres.

**Key Insights**
- Romance & Thriller show higher watch duration.  
- Music genre has highest completion rate.  
- Sci-Fi & Western show lower engagement depth.  

**Business Relevance**
- Prioritize high-performing genres  
- Improve underperforming categories  
- Strengthen personalization  

---

## 8. Netflix Originals Impact

**Columns Used**
- is_netflix_original  
- watch_duration_minutes  
- imdb_rating  
- monthly_spend  

**Purpose**  
To assess impact of original content.

**Key Insights**
- Engagement similar for originals & non-originals.  
- Originals slightly higher rated.  
- Revenue difference minimal.  

**Business Relevance**
- Originals improve brand perception  
- Cost-benefit analysis required  
- Maintain strong content catalog mix  

---

## 9. Age Group Segmentation

**Columns Used**
- Age_group  
- content_type  
- count of users  

**Purpose**  
To analyze demographic viewing patterns.

**Key Insights**
- Age group 26–50 drives majority of views.  
- Younger users prefer movies & series.  
- 50+ segment smaller but stable.  

**Business Relevance**
- Demographic targeting  
- Personalized marketing  
- Age-based recommendation strategy  

---

## 10. Churn Analysis

**Columns Used**
- is_active  
- watch_duration_minutes  
- progress_percentage  
- monthly_spend  

**Purpose**  
To understand behavioral differences between active and inactive users.

**Key Insights**
- Inactive users watch fewer minutes.  
- Inactive users spend less monthly.  
- Engagement directly influences retention.  

**Business Relevance**
- Early churn detection  
- Re-engagement campaigns  
- Retention-focused UX improvements  

---

## 11. Household Spending Power

**Columns Used**
- household_size  
- monthly_spend  
- watch_duration_minutes  

**Purpose**  
To evaluate monetization patterns across family sizes.

**Key Insights**
- Certain household sizes show higher average spend.  
- Larger households show high engagement but inconsistent spending.  

**Business Relevance**
- Design family bundle pricing  
- Identify account sharing risks  
- Develop multi-user subscription strategies  

---

## Overall Analytical Contribution

The pivot tables collectively provide:

- Revenue distribution analysis  
- Retention measurement  
- Engagement depth evaluation  
- Demographic segmentation  
- Content performance analysis  
- Monetization opportunity identification  

This pivot-based analysis converts raw streaming data into actionable business intelligence aligned with revenue growth and engagement optimization.
