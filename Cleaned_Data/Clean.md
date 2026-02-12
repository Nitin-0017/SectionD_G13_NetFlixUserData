# Data Cleaning Process

## Project:
User Engagement & Revenue Optimization Analysis for a Streaming Platform

---

## 1. Dataset

I started with the file https://drive.google.com/drive/folders/1cXwtUQGuZGUkcBEuCIxGHnYsLNm0CM8-?usp=sharing - Raw_Data.

After cleaning and filtering the data properly, the final dataset was reduced to around 5,000 valid rows.

- Cleaned_Data.csv (Google Sheet Link :- https://drive.google.com/drive/folders/1cXwtUQGuZGUkcBEuCIxGHnYsLNm0CM8-?usp=sharing - Cleaned_Data.

---

## 2. Handling Missing Values

I removed rows where important columns had missing values.

The columns checked were:

- imdb_rating  
- progress_percentage  
- watch_duration_minutes  
- monthly_spend  

These columns are very important for engagement and revenue analysis, so rows with null values in these fields were removed.

---

## 3. Data Filtering & Validation

To make sure the data is logical and clean, I applied the following rules:

- Removed users with age less than 18  
- Removed negative age values  
- Removed progress_percentage less than 0 or greater than 100  
- Removed watch_duration_minutes less than or equal to 0  
- Removed monthly_spend less than or equal to 0  

This helped remove incorrect and unrealistic values.

---

## 4. Columns Removed

Some columns had too many null values or were not useful for this project.

### Removed because of high null values or not relevant to problem:

- user_rating  
- genre_secondary  
- production_budget  
- box_office_revenue  
- number_of_seasons  
- number_of_episodes  

These columns were either incomplete or not required for engagement and revenue analysis.

---

### Removed because they do not support engagement or revenue analysis:

- session_id → too granular  
- user_id → personal identifier  
- movie_id → technical ID  
- email → personal data  
- first_name → personal data  
- last_name → personal data  
- state_province → too detailed geographic level  
- city → too granular  
- created_at → technical timestamp  
- content_warning → not used in KPIs  
- location_country → duplicate of country  
- primary_device → duplicate of device_type  
- subscription_start_date → not needed for this analysis  
- is_download → not relevant to engagement KPI  

These columns were removed to reduce unnecessary data and keep the dataset focused.

---

## 5. Final Dataset

The final cleaned dataset includes only the columns needed for:

- User engagement analysis  
- Revenue analysis  
- Subscription behavior  
- Content performance  
- Demographic insights  
