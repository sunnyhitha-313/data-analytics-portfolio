# **📸 Social Media Engagement & User Behavior Analytics (SQL)**
## **1️⃣ Problem Statement**

As a Data Analyst at Meta, the objective of this project is to collaborate with the Marketing team to leverage Instagram user data for:
* Increasing user engagement
* Improving retention
* Supporting influencer marketing
* Identifying growth opportunities
* Optimizing content strategy

The analysis focuses on extracting actionable insights from relational database tables to support data-driven marketing decisions.

## **2️⃣ Dataset Overview**

Database: ig_clone

**Tables Used:**
* users – registered user data
* photos – uploaded content
* comments – user interactions
* likes – engagement actions
* follows – network relationships
* tags – content categories
* photo_tags – tag mapping

The schema enforces primary and foreign key constraints ensuring data integrity.

## **3️⃣ Approach**
**Step 1: Data Validation**
* Checked for NULL values in all critical columns
* Verified duplicate records using GROUP BY + HAVING
* Confirmed schema-level constraints maintain integrity

**Step 2: Engagement Metrics Construction**

Key metrics created using JOIN, CTE, GROUP BY, and Window Functions:
* Total posts per user
* Total likes received
* Total comments received
* Engagement per post
* Total engagement (likes + comments)
* follower count & following count
* Hashtag engagement performance
* Cohort-based engagement (joining year)
* User segmentation categories

**SQL techniques used:**
* CTEs
* CASE statements
* RANK() / DENSE_RANK()
* COALESCE()
* NULLIF()
* NOT EXISTS

## **4️⃣ Key Insights & EDA Findings**
### **📊 User Activity Distribution**
* 74% of users are active
* 26% are completely inactive

A quarter of the platform does not contribute to engagement or content creation, representing a major retention opportunity.

### **📈 Engagement Concentration**
* Engagement is highly concentrated among a small group.
* Top 10 users generate over 200 interactions each.
* Highest performer reaches 405 total engagements.
  
Platform engagement follows a power-law distribution driven by top creators.

### **🏷 Hashtag & Content Insight**
* #smile generates the highest engagement (1802 interactions).
* Lifestyle and emotion-based hashtags dominate performance.
* Content themes strongly influence interaction levels.

Emotion-driven and visually appealing content drives the highest engagement.

### **📤 Upload vs Engagement Correlation**
* Engagement increases consistently with posting frequency.
* Users with 1–2 posts average below 110 interactions.
* Users with 5+ posts exceed 200 average engagements.
* Users with 12 posts reach average engagement of 749.

Consistency significantly amplifies audience interaction.

### **👥 Cohort Analysis (Joining Year)**
* 2016 users: Avg 51.43 engagement per post
* 2017 users: Avg 48.9 engagement per post

Engagement efficiency remains stable across cohorts, indicating consistent platform experience over time.

### **🧩 User Segmentation Model**

Users segmented based on posting activity and engagement efficiency:
* 53% Emerging Users
* 19% High-Value Creators
* 26% Inactive Users
* 2% Active Low-Engagement Users

Emerging Users represent the largest growth opportunity.

### **🌟 Influencer & High-Value Creator Identification**
**Selection Criteria:**
* Minimum 5 posts
* Engagement per post > 35
* Strong total engagement consistency

**Key Insight:**

Engagement per post is a stronger influencer metric than follower count.

High-efficiency creators average above 42 interactions per post.

### **🏅 Brand Ambassador Identification**

Ambassador Criteria:
* Minimum 8 posts
* Engagement per post ≥ 35
* Total engagement > 300

These users demonstrate long-term consistency and stable audience interaction, making them reliable for platform initiatives.

## **5️⃣ Model Performance**

No predictive models were implemented.

All insights are derived using:
* SQL-based aggregation
* Relational joins
* Cohort comparison
* Ranking functions
* Segmentation logic
* Behavioral pattern analysis

## **6️⃣ Architecture / Analysis Flow**

Raw Relational Tables

→ Data Validation

→ Metric Engineering (Engagement KPIs)

→ Aggregation & Ranking

→ Segmentation Modeling

→ Marketing Strategy Framework

→ Business Recommendations

## **7️⃣ Strategic Growth Framework**
**🔁 Retention Strategy**
* Reactivate 26% inactive users
* Personalized notifications
* Gamification incentives

**📈 Growth Strategy**
* Convert Emerging Users (53%) into High-Value Creators
* Encourage posting consistency
* Promote high-performing hashtags

**⚡ Engagement Optimization**
* Reward high-efficiency creators
* Prioritize emotion-driven content themes
* Track engagement per post as a core KPI

## **8️⃣ Business Recommendations**
* Prioritize reactivation of inactive users
* Develop structured influencer programs using engagement efficiency
* Encourage consistent content creation
* Invest in Emerging Users as scalable growth segment
* Use cohort-based lifecycle marketing
* Implement KPI tracking using engagement per post

## **9️⃣ Future Improvements**
* Incorporate ad campaign data (CTR, conversion rate, ROAS)
* Build dashboard visualization (Power BI / Tableau)
* Implement churn prediction modeling
* Add time-based engagement trend analysis
* Develop automated influencer scoring system
