
# **Title:**

# **User Engagement & Revenue Optimization Analysis for a Streaming Platform**

# **Sector:**

# Media & Entertainment / Digital Streaming

# **Team Details:**

Section-D G-13

1\.  Palak Gupta (Project Lead)  
2\.  Piyush Raj  
3\.  Nitin Kumar  
4\.  Abhijeet   
5\.  Pratyaksha Shastri  
6\.  Keshav Goel

## Problem

## Streaming platforms generate large volumes of user interaction data, but without structured analysis, it becomes difficult to identify what truly drives user engagement, retention, and subscription revenue. Decisions related to content strategy, subscription pricing, and user experience often rely on assumptions rather than evidence-based insights.

The key challenge addressed in this project is to **understand which user behaviors, subscription plans, and content characteristics most strongly influence engagement and revenue**, and how these insights can be used to improve retention and monetization for a digital streaming platform.

## Approach

To address this problem, a simulated streaming platform dataset was analyzed using Google Sheets. The raw dataset initially contained over 10,000 records and numerous columns with missing, inconsistent, or irrelevant values.

The approach followed four major steps:

1. **Data Cleaning & Preparation**

   * Removed columns with high missing values or low business relevance

   * Handled missing values using mode and median imputation

   * Standardized categorical values (country, device type, subscription plan)

   * Converted columns into appropriate data types

   * Final cleaned dataset contained **5,025 rows and \~20 analytical columns**

2. **Feature Selection**  
    Focused on columns supporting engagement and revenue analysis, including:

   * Watch duration, completion percentage  
     Subscription plan, monthly spend, active status  
   * Content type, genre, IMDb rating

   * Demographic attributes such as age, gender, and country

3. **Pivot-Based Analysis**  
    Multiple pivot tables were created to analyze:

   * Revenue by subscription plan

   * Engagement by device and content type

   * Retention patterns across user segments

   * Genre-level engagement depth

4. **Dashboard Creation**  
    Insights were consolidated into an interactive dashboard to enable quick comparison, filtering, and executive-level decision making.

## Key Insights

* **Engagement and retention are strongly correlated**: Active users consistently show higher watch duration and completion percentages compared to inactive users.

* **Premium subscription tiers generate the highest total revenue**, while some mid-tier plans show strong average spend per user.

* **Content type influences engagement**: Movies generate the highest view volume, while series and documentaries show deeper engagement.

* **Device usage impacts watch behavior**: Desktop and tablet users demonstrate slightly higher watch duration compared to mobile users.

* **Geographic concentration exists**: A small number of countries contribute a majority of platform revenue, indicating regional dependency.

* **Netflix Originals improve content perception**, though revenue differences between original and non-original content are marginal.

# **Sector & Business Context:**

Sector Overview  
The project is based in the **Digital Entertainment & Streaming Services** sector. Streaming platforms such as Netflix, Amazon Prime, and Disney+ operate on subscription-based business models where user engagement, retention, and content consumption directly impact revenue growth. These platforms rely heavily on data analytics to understand viewer behavior and optimize content offerings at scale.

Current Challenges  
High competition leading to **subscriber churn**

Difficulty identifying **which user behaviors drive long-term engagement**

Balancing revenue growth across different **subscription tiers**

Understanding how **demographics and devices** influence consumption behavior

Why this Problem was chosen 

This problem was selected because **user engagement and revenue optimization are critical to the sustainability of streaming platforms**. By analyzing user behavior, subscription plans, and content performance together, the project aims to uncover actionable insights that support:

* Better content strategy decisions

* Improved user experience

* Increased retention and monetization

**Data Description**

Dataset Source

The dataset used in this project is **“Netflix 2025: User Behavior Dataset (210K+ Records)”**, sourced from **Kaggle**.  
**Access link:**  
[https://www.kaggle.com/datasets/sayeeduddin/netflix-2025user-behavior-dataset-210k-records](https://www.kaggle.com/datasets/sayeeduddin/netflix-2025user-behavior-dataset-210k-records)

Data Structure

The raw dataset consists of multiple CSV files capturing:

* User demographics and subscription details

* Content metadata

* User watch and engagement behavior

For this project, the data was cleaned and consolidated into a single analysis-ready table.

### Key Columns Used

### **User & Demographics:** age, gender, country, household\_size **Engagement:** watch\_duration\_minutes, progress\_percentage, device\_type, watch\_date **Revenue:** subscription\_plan, monthly\_spend, is\_active **Content:** genre\_primary, content\_type, imdb\_rating, release\_year, is\_netflix\_original

### Data Size

Initial sample: \~10,000 rows  
Final cleaned dataset: **5,025 rows**  
Final columns used: **\~20 analytical columns**

Data Limitations

Dataset is simulated and may not fully represent real Netflix user behavior  
No explicit churn date is available; retention is inferred using activity status  
Financial metrics are limited to subscription spend only

**Data Cleaning and Preparation**

Missing Values Handling

* All data cleaning and transformation steps were performed entirely in Google Sheets, in accordance with the capstone project requirements.  
* Columns with excessive missing values and low analytical relevance were removed.

* Missing values in key demographic fields were handled using:

  * **Mode imputation** for gender

  * **Median imputation** for household size

* Rows were not dropped unnecessarily to preserve dataset size and distribution.

Outlier Treatment

* Invalid and extreme values (such as unrealistic ages or negative durations) were filtered out.

* No aggressive trimming was applied to avoid biasing user behavior patterns.

Transformations

* Text standardization was applied to categorical columns (country, device type, subscription plan).

* Boolean fields were normalized to consistent TRUE/FALSE values.

* Date fields were converted to proper date formats for time-based analysis.

Feature Engineering

* A derived **maturity\_level** column was created from content rating for better audience segmentation.

* Age groups were created to support demographic analysis.

* Engagement and revenue-ready numeric fields were formatted appropriately.

Assumptions

* User activity status (is\_active) was used as a proxy for retention.

* Monthly subscription spend was assumed to represent user revenue contribution.

* Engagement was measured using watch duration and completion percentage.

All data cleaning and transformation steps were performed entirely in Google Sheets, in accordance with the capstone project requirements.

##  Dashboard View Structure

The dashboard is structured into clearly separated sections for intuitive navigation:

1. **Top KPI Section**

   * Total Revenue

   * Average Monthly Spend

   * Active User Count

   * Average Watch Duration

2. **Revenue & Retention Analysis**

   * Revenue by Subscription Plan (Bar Chart)

   * Active Rate by Subscription Plan (Horizontal Bar Chart)

3. **Engagement Analysis**

   * Watch Duration by Device Type

   * Engagement by Content Type

4. **Distribution Analysis**

   * Revenue by Country

   * Top 5 Genres by Engagement

5. **Behavioral Comparison**

   * Churn Comparison (Active vs Inactive Users)

   * Engagement vs Monthly Spend

This layout allows users to move from **high-level KPIs to detailed behavioral insights** smoothly.

## Filters & Drilldowns

To enable interactive exploration, the dashboard includes slicers and filters such as:

* Subscription Plan

* Country

* Device Type

* Content Type

* Active Status

These filters allow stakeholders to:

* Compare performance across user segments

* Drill down into specific regions or subscription tiers

* Analyze engagement patterns for targeted decision-making

All charts update dynamically based on filter selection.
