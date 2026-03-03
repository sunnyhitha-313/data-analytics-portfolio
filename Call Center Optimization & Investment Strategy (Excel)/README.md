# **📞 Call Center Optimization & Investment Strategy**
## **1️⃣ Problem Statement**

AstroSage received a ₹1 Crore investment to improve its call center operations.

The objective of this project is to analyze historical consultation data (calls & chats) to identify:
* Operational inefficiencies
* Call completion issues
* Agent workload imbalance
* Customer satisfaction gaps
* Revenue concentration risks
  
The goal is to provide data-driven recommendations for allocating the ₹1 crore investment to improve efficiency, service quality, and profitability.

## **2️⃣ Dataset**

* Total Records: 28,027
* Raw Columns: 35
* Cleaned Columns: 32
* Total Days Analyzed: 34
* Total Calls: 8,508
* Total Chats: 19,514
* Total Gurus: 148
* Total Net Revenue: ₹2,13,987.32
* Overall Average Rating: 2.93

### **Data Includes:**

* Session IDs (_id, uid, gid)
* Consultation Type (Call / Chat / Complimentary / Public Live Call)
* Call & Chat Status
* Duration Metrics
* Financial Metrics (amount, netAmount, astrologersEarnings)
* Customer Ratings
* Platform (App, Dashboard, GuruCool)
*Time-Based Fields (Date, Month, Hour)

## **3️⃣ Approach**
**Step 1 – Data Cleaning**
* Removed duplicate records
* standardized date-time fields
* Converted financial & duration columns to numeric
* Derived Date, Month, Hour, Month-Year
* Cleaned inconsistent categorical values

**Step 2 – Aggregation & Analysis**

**Used:**
* Pivot Tables
* COUNT
* SUM
* AVERAGE
*CORREL
*Bar & Column Charts

**Analysis Dimensions:**
* Daily & Hourly Trends
* Revenue by Consultation Type
* Platform Performance
* Call Status Distribution
* Rating Distribution
* Guru-wise Workload
* Repeat Caller Analysis

## **4️⃣ EDA Insights**
### **📊 Call Volume & Demand**
* Average Daily Calls ≈ 250
* Highest Daily Calls: 430
* December Calls: 8,090
* January Calls: 418
* Call volume fluctuates significantly, indicating unstable demand patterns.

### **📉 Call Completion Crisis**
* Out of 8,508 calls:
* Completed: 3,450 (40.55%)
* Failed / Busy / No Answer / Incomplete: 59.45%
  
More than half the calls fail.
This is the biggest operational weakness.

### **💰 Revenue Analysis**
* Calls contribute ≈ 79% of total revenue
* Chats contribute ≈ 21%
* Calls are the core profit engine

If call performance improves → profitability improves directly.

### **⭐ Customer Satisfaction**
* Overall Rating: 2.93
* Call Rating: 3.50
* Chat Rating: 2.69
* Complimentary: 4.5

Majority of ratings fall in lower ranges.

Duration does not strongly correlate with satisfaction.

### **🔁 Repeat Customer Strength**
* Repeat Callers: 1,272
* Calls by Repeat Users: 6,156
* Repeat Contribution: 72.36%

Strong user dependency — but risky if service quality drops.

### **👥 Workload Imbalance**
* Average Calls per Guru ≈ 66
* Some gurus handled 1,000+ calls
* Many handled fewer than 10

Workload distribution is heavily skewed.

Burnout risk is high.

### **⏰ Peak Hour Pressure**

Peak demand between:
* 7 AM – 11 AM
* 2 PM – 4 PM

Peak-hour overload directly increases call failures.

### **📈 Revenue–Agent Correlation**
Correlation between astrologer earnings and net revenue ≈ 0.99
Agent performance directly impacts company income.

## **5️⃣ Model Performance**
No predictive or machine learning models were implemented.

All insights are derived using:
* Aggregation-based analysis
* Statistical correlation
* Trend comparison
* Pivot-based KPI evaluation

## **6️⃣ Architecture (Process Flow)**

Raw Dataset

→ Data Cleaning

→ Feature Engineering (Time & Financial Fields)

→ Pivot-Based Aggregation

→ Visualization

→ Dashboard

→ Strategic Investment Allocation

## **7️⃣ Demo / Dashboard**

**The final Excel dashboard includes:**

**🔹 KPIs**
* Total Revenue
* Total Calls
* Total Chats
* Total Gurus
* Average Rating
* Average Calls per Agent

**🔹 Operational Metrics**
* Call Status Distribution
* Chat Status Distribution
* Hourly Call Distribution
* Day-wise Call Trend

**🔹 Performance Metrics**
* Top Gurus by Calls
* Guru-wise Rating
* Category-wise Revenue
* Platform-wise Revenue & Rating

**🔹 Filters**
* Consultation Type
* Year
* Platform

## **8️⃣ Strategic Investment Allocation (₹1 Crore Plan)**
**30% – Technology Upgrade (₹30 Lakhs)**
* Intelligent routing
* Infrastructure scaling
* Reduce busy/failed calls
* Improve call completion rate
  
**25% – Workforce Expansion (₹25 Lakhs)**
* Hire additional agents
* Shift-based scheduling
* Peak-hour staffing
* 20% – Training Programs (₹20 Lakhs)
* Communication skill improvement
* Service quality monitoring
* Standardized consultation process
  
**15% – Customer Experience Optimization (₹15 Lakhs)**
* Queue optimization
* Feedback analysis
* Loyalty programs
* 10% – Revenue Growth Strategy (₹10 Lakhs)
* Promote high-revenue categories
* Bundle services
* Demand stabilization campaigns

## **9️⃣ Future Improvements**
* Implement demand forecasting using time-series analysis
* Build Power BI interactive version
* Introduce churn prediction model
* Automate workload balancing algorithm
* Integrate CRM analytics for personalization
