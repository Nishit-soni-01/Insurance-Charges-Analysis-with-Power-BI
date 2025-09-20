# Insurance-Charges-Analysis-Dashboard

### Dashboard Link: [Insert Your Power BI Report Link Here]

## Problem Statement

This dashboard provides a detailed analysis of medical insurance charges to identify the key factors that influence costs for policyholders. By visualizing data related to demographics and lifestyle choices, the report helps stakeholders understand the primary drivers behind insurance premiums. The key objectives are to determine the impact of smoking, age, BMI, and region on charges, enabling better risk assessment and more informed business decisions for the insurance provider.

### Steps Followed

-   **Step 1:** Loaded the dataset (`InsuranceData.csv`) into Power BI Desktop.
-   **Step 2:** Opened the Power Query Editor to check data quality, column types, and handle any missing values.
-   **Step 3:** In the report view, a clean and professional theme was selected for optimal data visualization.
-   **Step 4:** Added interactive **Slicers** to the report for `Region` and `Number of Children` to allow for dynamic data filtering.
-   **Step 5:** Created three core DAX measures to serve as Key Performance Indicators (KPIs).
    ```dax
    Total Charges = SUM(InsuranceData[charges])
    ```
    ```dax
    Average Age = AVERAGE(InsuranceData[age])
    ```
    ```dax
    Average BMI = AVERAGE(InsuranceData[bmi])
    ```
-   **Step 6:** Added **Card** visuals to the canvas to display the main KPIs: "Total Charges," "Average Age," and "Average BMI."
-   **Step 7:** Designed the main dashboard with a variety of visuals to explore the data:
    -   A **Donut Chart** to show the breakdown of "Charges by Smoker."
    -   A **Clustered Bar Chart** to compare "Charges by Sex & Smoker."
    -   An **Area Chart** to illustrate the trend of "Charges by Age."
    -   A **Map** visual to show the geographical distribution of "Charges by Region."
    -   A **Donut Chart** to visualize "Charges by Children."
-   **Step 8:** The final report was published to the Power BI Service for easy access and sharing.

---

# Snapshot of Dashboard
<img width="1303" height="731" alt="Screenshot 2025-09-20 185418" src="https://github.com/user-attachments/assets/faa757a1-18c8-406e-baaa-6c4b2d5042e8" />
<img width="1367" height="737" alt="Screenshot 2025-09-20 185407" src="https://github.com/user-attachments/assets/f8297588-a148-4dc5-b2a2-c540e10a9947" />
<img width="1332" height="718" alt="Screenshot 2025-09-20 185426" src="https://github.com/user-attachments/assets/bd4d395f-68a7-43c6-8ac9-4d834706e335" />



---

# Insights

This dashboard reveals several critical insights into the factors driving medical insurance charges.

### [1] Key Metrics Overview

-   **Total Charges:** \$8.8 Million
-   **Average Age of Policyholder:** 39 years
-   **Average BMI of Policyholder:** 30.66
    -   *Note: An average BMI above 30 is typically classified as obese, indicating a significant health factor across the policyholder base.*

### [2] The Impact of Smoking is a Primary Driver

-   Smokers account for a vastly disproportionate amount of total insurance charges compared to non-smokers. This highlights **smoking status as the single most significant predictor** of high medical costs.

### [3] Charges Increase with Age

-   The area chart shows a clear and strong positive correlation between age and insurance charges. Costs rise steadily as policyholders get older, with significant increases in later years.

### [4] Geographical & Family Factors

-   **Regional Differences:** The map shows that total charges vary by region, with certain areas having higher overall medical costs.
-   **Impact of Children:** The number of children a policyholder has also influences the total charges, though to a lesser extent than smoking or age.
