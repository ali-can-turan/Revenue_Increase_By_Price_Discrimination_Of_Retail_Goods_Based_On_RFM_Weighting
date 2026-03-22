Price Discrimination: Revenue Optimization through RFM & WTP Modeling

This project implements a Price Discrimination Strategy aimed at maximizing retail revenue using RFM Analysis and Willingness to Pay (WTP) modeling.
By segmenting customers based on their purchasing behavior, updated pricing tiers were simulated to achieve a significant revenue jump.

<img width="1192" height="172" alt="Revenue Change-2" src="https://github.com/user-attachments/assets/86533b04-3c50-41b6-9d55-12f9b4ca8cae" />


📊 Business Impact
Total Revenue Increase: 7.5%
Net Revenue Change: +35,542.09

<img width="1026" height="433" alt="Revenue change by stock" src="https://github.com/user-attachments/assets/0ad5ac9b-d83a-4389-abd9-95cdd922bc96" />

[View dashboard for all insights (pdf)](Online_Retailer_II_DB.pdf)

[View all the details, insights and steps through this project (docx)](readMe_extensive.docx)

[View cleaned and filtered data used in this project (xlsx)](online_retail_II_cleaned_and_filtered.xlsx)

[View original data in cleaned version (xlsx)](online_retailer_II_original_cleaned.xlsx) 


Core Logic: 
Leveraged high-value customer segments (Champions & Loyalists) to implement premium pricing while offering discounts to retain "Hibernating", "At Risk" and "Potential Loyalist" segments.

🛠️ Tech Stack & MethodologyData Source: Online Retailer II (Kaggle)

Tools:
* Microsoft Excel: Data cleaning, RFM calculation, and WTP normalization.
* IBM Cognos Analytics: Data modeling (Calculated Fields), Dashboarding, and Storytelling.

Framework:
* RFM Formula: R * 0.2 + F * 0.4 + M * 0.4.
* Customer Surplus Proxy: Integrated a binary "Above Average Price" flag to refine WTP values.

<img width="1086" height="241" alt="RFM" src="https://github.com/user-attachments/assets/9e73f38f-143a-4623-9466-45651bc4796b" />

🧹 Key Data Engineering StepsFiltering: Focused on the United Kingdom to avoid outlier distortion and selected the top 10 recurring products for deep analysis.

Cleaning: Removed nulls, duplicates, and non-positive quantity/price entries.

Enrichment: Separated date fields and applied Min-Max Normalization to RFM scores.

<img width="1777" height="181" alt="Fitered_Cleaned" src="https://github.com/user-attachments/assets/7a2ff139-d560-423f-a944-601f805ba643" />


📈 Key Insights: Segment Power: 
* Champions represent 48.6% of the customer base, providing the safest ground for price adjustments.
* Potential Loyalists: While fewer in number, they tend to purchase higher-priced items compared to other segments.
* Product Performance: Stock code 22423 emerged as the primary revenue driver post-optimization.

<img width="1024" height="580" alt="Ekran görüntüsü 2026-03-22 171244" src="https://github.com/user-attachments/assets/556dafe9-0da6-4446-9eb1-71bb2bca25ac" />


📝 Assumptions & Future Work

Assumption: The model assumes that WTP modeling accurately predicts consumer surplus such that demand quantity remains constant despite price changes.

Future: Implementing Regression Analysis to validate the reliability of individual customer revenue contributions.
Future: Replacing proxy models with Price Elasticity analysis once more granular price transition data is available.
