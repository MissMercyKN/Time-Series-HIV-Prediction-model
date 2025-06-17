# Time-Series-HIV-Prediction-model
📌 Title:
HIV Infection Rate Forecasting and Analysis (2000–2026) to Support SDG 3: Good Health and Well-being

Introduction – The SDG Challenge
The Sustainable Development Goal 3 (SDG 3) calls for ensuring healthy lives and promoting well-being for all. One of its targets is to end the epidemic of AIDS by 2030. Despite major progress, HIV remains a serious public health concern in many regions, especially sub-Saharan Africa.

Understanding the trend and future projections of HIV infection rates is critical for public health planning and timely intervention.

The Data Science Solution
My project leverages historical HIV infection data across different demographics (age, sex, and location) to analyze and forecast future infection trends using machine learning.

I used Facebook Prophet, a time series forecasting model developed by Meta. It is robust to outliers, can model seasonality, and performs well on public health data with yearly trends.

The dataset spans from 2000 to 2019, and forecasts were generated up to 2026.

📊 Data Description:
Source: UN SDG Dataset

Period: 2000–2019 (forecasted to 2026)

Indicators: New HIV infections per 1,000 uninfected population

Dimensions: Geographic Area, Sex, Age, Year

🧹 Data Cleaning Summary:
Removed unnecessary columns like “Footnotes”, “ObjectId”, etc.

Melted wide “Value year” columns into long format (Year, HIV_Infection_Rate)

Removed 27 rows with missing values

Renamed final dataset to df_clean for clarity

🔍 Exploratory Data Analysis (EDA):
Trends: HIV infection rates show a general decline from 2000 to 2019.

Distribution: Most values lie between 0 and 5, with some outliers above 50.

Group Insights: Infection rates vary by sex and age, with some demographic patterns emerging.

Heatmap & Boxplots: Highlighted variability and central tendency across years and sexes.

📈 Forecasting Approach:
Tool Used: Facebook Prophet

Data Aggregated: Average infection rates per year

Forecast Horizon: Up to 2026

Confidence Interval: 95%

📌 Key Insights:
Forecast indicates that HIV rates will remain stable or slightly decline beyond 2025.

Intervention efforts appear effective; however, variations across sex/age groups suggest targeted campaigns are still needed.

Forecast range is narrow, indicating model confidence in stability.

Ethical Considerations
⚠️ Bias Awareness: The dataset may underrepresent marginalized groups or regions.

🔐 Privacy: No personal identifiers were used or exposed.

🤝 Actionability: Forecasting is not a replacement for real-world efforts but a decision-support tool.

✅ Conclusion:
This analysis confirms a consistent downward trend in HIV infections. With continued public health efforts, rates are likely to stabilize through 2026. Future work could explore regional comparisons or evaluate intervention impacts over time.

📂 Next Steps / Recommendations:
Integrate location-level analysis to pinpoint hotspots

Compare with ART (antiretroviral treatment) access data

Re-validate model annually with updated data

