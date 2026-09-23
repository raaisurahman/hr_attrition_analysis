## 📊 HR Attrition Analysis (IBM Dataset)
An end-to-end data analytics solution built in Microsoft Fabric to uncover employee turnover drivers and empower secure, data-driven retention strategies.

## Purpose

This HR Attrition Analysis dashboard is an interactive analytical tool designed to help HR professionals and department heads understand why employees leave. By ingesting and analyzing 1,470 employee records, the report identifies key attrition drivers across different departments, salary bands, and age groups. It empowers leadership to make informed retention decisions while ensuring strict data privacy and governance through dynamic row-level security.

## Tech Stack

The dashboard and its underlying architecture were built using the following tools and technologies:

*  **Microsoft Fabric** – End-to-end analytics platform used for hosting and managing the overarching data architecture.
*  **Dataflows Gen2** – Used as the ingestion layer to process and load the 1,470 employee records.
*  **Power BI** – Main data visualization platform used for report creation and interactive analysis.
*  **DAX (Data Analysis Expressions)** – Utilized for calculated measures and to implement dynamic Row-Level Security (RLS) using the `USERPRINCIPALNAME` function.
*  **Data Governance & Security** – Applied Confidential sensitivity labels to protect personal data and ensure compliance.

## 4. Data Source

**Source:** IBM HR Analytics Employee Attrition & Performance Dataset.
The dataset consists of 1,470 employee records containing comprehensive attributes covering demographics, job characteristics, compensation, and historical performance. Key structured columns include: `Age`, `Attrition`, `BusinessTravel`, `DailyRate`, `Department`, `DistanceFromHome`, `Education`, `EducationField`, `EnvironmentSatisfaction`, `Gender`, `HourlyRate`, `JobInvolvement`, `JobLevel`, `JobRole`, `JobSatisfaction`, `MaritalStatus`, `MonthlyIncome`, `NumCompaniesWorked`, `OverTime`, `PercentSalaryHike`, `PerformanceRating`, `RelationshipSatisfaction`, `TotalWorkingYears`, `TrainingTimesLastYear`, `WorkLifeBalance`, `YearsAtCompany`, `YearsInCurrentRole`, `YearsSinceLastPromotion`, and `YearsWithCurrManager`.

##  Highlights

* **Business Problem**
High employee turnover costs companies time, resources, and institutional knowledge. HR and department leaders often lack visibility into *who* is leaving and *why*. Without granular insights into compensation, departmental trends, and demographics, retention strategies are based on guesswork. Furthermore, sharing sensitive HR data across a large organization poses security risks if department heads can view salary and performance data outside their own teams.
* **Goal of the Dashboard**
To deliver a secure, interactive visual tool that highlights key attrition drivers and enables deep-dive exploratory analysis across multiple employee variables. It is designed to support strategic retention planning while enforcing strict data access controls so managers only view their respective teams.

## Walkthrough of Key Visuals

* **Key KPIs (Top Ribbon):** Instantly track Overall Attrition Rate (16.12%), Total Employees Left (237), Total Headcount (1,470), Average Monthly Income (6,503), and the Avg Tenure of Leavers (5.13 years).


* **Dynamic Filtering:** Interactive slicers allow users to filter the entire report by Department, Gender, and Salary Band, with dedicated buttons to seamlessly toggle between the high-level "Overview" and granular "Deep Dive" pages.


* **Attrition Decomposition Tree:** A visual breakdown analyzing attrition paths dynamically by Department, filtering down into specific Job Roles and Salary Bands to find root causes.


* **Department & Role Analysis:** Horizontal bar charts and detailed matrix tables outline attrition percentages across different business units (e.g., Sales, Research & Development) and specific job roles (e.g., Sales Executive, Laboratory Technician).


* **Demographic & Lifestyle Deep Dive:** Dedicated visualizations displaying attrition segmented by Age Group, Education Field, Marital Status, and Business Travel frequency, utilizing colors to highlight high-risk categories (e.g., the 18 to 25 age bracket and the "Under 3k" salary band).




## Business Impact & Insights

* **Targeted Retention Programs:** By surfacing distinct attrition drivers across age groups and salary bands, HR can pinpoint high-risk segments (such as newer, lower-income employees) and implement proactive, targeted retention initiatives.
* **Secure Data Governance:** The implementation of dynamic row-level security (RLS) ensures that department heads can safely interact with the dashboard to manage their own teams without exposing confidential, cross-departmental HR data.
* **Strategic Policy Adjustments:** Insights into how business travel frequency or specific departments correlate with turnover can inform better recruitment strategies, expectation-setting, and work-life balance policies.

### Screenshots 
Here is the screenshot of the dashboard after published in Fabric.
 ![Dashboard Preview](https://github.com/raaisurahman/hr_attrition_analysis/blob/main/snapshot%20of%20dashboard's%20deepdive%20page.png)
 ![Dashboard Preview](https://github.com/raaisurahman/hr_attrition_analysis/blob/main/snapshot%20of%20dashboard's%20overview%20page.png)
