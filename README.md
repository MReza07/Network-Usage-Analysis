📡 Network Usage Analysis – Power BI Dashboard

This project provides an in-depth analysis of telecom network usage, customer data consumption patterns, revenue trends, and service performance metrics. The dashboard helps identify high-value regions, network performance gaps, and customer satisfaction drivers to support data-driven decision-making.

🖼 Dashboard Screenshot https://github.com/MReza07/Network-Usage-Analysis/tree/main/schreenshots

📊 Dashboard Overview

✔ Usage Insights by Region

Identify high-consumption regions like Dhaka and Chittagong and track regional usage distribution.

✔ Network Type Performance

Compare data usage and speed across 3G, 4G, and 5G networks.

✔ Customer Satisfaction

Understand how satisfaction levels impact data usage and service performance.

✔ Revenue Trends

Monitor monthly revenue patterns to detect growth opportunities or declining phases.

✔ Speed Analysis

Visual breakdown of average speed contribution by network type.


## 📐 Sample DAX Measures   

MoM Growth % = 
VAR PrevMonth = CALCULATE([T_Data_Use], DATEADD('Date_Master'[Date], -1, MONTH))
RETURN
DIVIDE([T_Data_Use] - PrevMonth, PrevMonth) * 100

avg_Revenue = AVERAGE(Network_Usage_Data[TotalRevenue])

all_customer = COUNTROWS(Network_Usage_Data)

Total Revenue (Previous Month) = 
CALCULATE([T_Revnnue], DATEADD('Date_Master'[Date], -1, MONTH))

🛠 Tools & Technologies

Tool	Purpose

Power BI	Data modeling, DAX measures, visualization

Excel / CSV	Raw dataset preparation

Power Query	Data cleaning & transformation

DAX	Calculated fields and business metrics

📁 Project Structure

📦 Network Usage Analysis
│
├── 📄 Dataset/

│     └── Network_Usage_Dataset.xlsx
│
├── 📄 PBIX/

│     └── network usage data.pbix
│
├── 📄 Screenshots/

│     ├── Network Usage Data analysis Report.PNG

│     ├── Average Data Usage bt Region.PNG

│     ├── Average Data Usage by Network.PNG

│     └── Average Data Usage by Region.PNG
      └──  Average Speed by Network .PNG
│
└── 📄 README.md


 📥 How to Open the Report

Download the PBIX file

Network_Usage_Analysis.pbix

Open in Power BI Desktop (latest version recommended)

Refresh the dataset if needed.

🔍 Key Insights (From the Dashboard)

Customer data usage and engagement remain strong, driving 1.48M total revenue.

5G users show the highest usage and speeds, especially in metro regions.

Network performance is stable with 0.80% downtime, supporting higher satisfaction.

Monthly revenue shows a gradual decline, indicating potential customer churn or seasonal effect.

Lower-usage regions present opportunities for promotional or retention strategie

📚 Learning Outcomes

Telecom KPI analysis

DAX measures for performance metrics

Advanced Power Query data transformations

Region-wise performance comparison

Customer satisfaction correlation analysis

## 📜 License

This project is released under the MIT License.


## 📬 Contact

Md. Rezaul Repon

Data Analyst (Power BI | SQL | Python)

🔗 GitHub: https://github.com/MReza07

📧 Email: reazulrepon@gmail.com



