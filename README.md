<img width="1357" height="380" alt="IBM teleco Churn Dahsboard" src="https://github.com/user-attachments/assets/b5ded319-bdbd-4376-ad43-cefd22d86f35" />


# 📊 Telecom Customer Churn & Retention Analytics Dashboard
### Strategic Revenue Optimization and Attrition Diagnostics (IBM Corporate Case Study)

## 🎯 Project Overview & Executive Summary
This project analyzes customer loss (attrition) for a major telecommunications provider using a tracking database of over 7,000 customers. The objective was to audit customer billing data, uncover the true root causes of customer loss, evaluate product packages, and calculate the exact financial damage to the business.

The company is currently facing a major customer retention issue with an overall **churn rate of 26.54%**—which has resulted in a massive **$2,862,926.90 in lost historical revenue**. This deep-dive analysis reveals that the loss is driven by three main areas: customer support friction, digital billing hurdles for seniors, and low-engagement service accounts. This dashboard provides business leaders with a clear, data-driven roadmap to fix customer service issues, protect high-value accounts, and stop ongoing revenue loss.

---

## 🧼 Data Auditing & Cleaning Process (Ensuring Business Accuracy)

Before creating any charts or summaries, a complete data audit was performed in Microsoft Excel. This step ensures that all financial and customer metrics are 100% accurate before business decisions are made.

### 1. Correcting Hidden Blanks in Total Charges
* **The Business Issue:** The `TotalCharges` column contained 11 hidden blank cells that broke formulas and caused calculation errors.
* **The Root Cause:** Investigation showed these rows belonged to brand-new customers who had a tenure of `0` months. Because they were in their very first billing cycle, they had not generated historical charges yet.
* **The Business Fix:** Discovered these accounts using Excel's Filter tool, updated the blank spaces to a proper numeric value of `0.00`, and formatted the column as *Currency ($)*. This preserved accurate tracking without distorting company financial records.

### 2. Making Customer Labels Readable
* **The Business Issue:** Crucial data points like `SeniorCitizen` were originally recorded as system codes (`1` and `0`), which would look confusing on a final executive report or filter.
* **The Business Fix:** Used Excel's **Find and Replace** tool to change `1` to `"Senior"` and `0` to `"Non-Senior"`, making the final dashboard instantly easy to read for any manager.

### 3. Creating Custom Business Categories
To uncover deeper business trends, two custom tracking columns were built using Excel formulas:
* **`Total Add-ons` Column:** Built using the `=COUNTIF()` formula to instantly count how many extra premium services (like Online Security or Tech Support) a customer purchased. This allows us to see how product combinations affect loyalty.
* **`Customer Value Tier` Column:** Built using the `=PERCENTILE.INC()` formula to automatically isolate the top 10% highest-value customers based on their predicted lifetime financial value (`CLTV`). This ensures the business can identify and protect its most critical clients.

---

## 🛠️ Data Glossary (Metrics Explained)

* **Historical Revenue Lost:** The total lifetime money spent by customers who have already canceled and left the company.
* **High-Value Customer (HVC):** Elite accounts ranking in the top 10% of predicted customer lifetime value.
* **Revenue Risk (CLTV):** The estimated future financial value at stake from active high-value customers who are currently showing signs of leaving.
* **Service Bundling Power:** The total number of premium extra services a customer has active (ranging from 0 to 6).

---

## 🔎 The 5 Key Business Challenges & Insights Uncovered

### Challenge 1: Overall Churn & Financial Loss
* **The Goal:** Measure the true financial impact and scale of customer loss across the whole company.
* **The Data:** The overall customer loss rate is **26.54%**, costing the company **$2,862,926.90** in lost historical revenue.
* **Key Business Insight:** Losing more than a quarter of your entire customer base is a major business threat. The company cannot fix this problem just by spending money to acquire new customers; keeping current customers must become the top priority.

### Challenge 2: Technical Support Friction & Digital Care
* **The Goal:** Uncover how offering technical support affects customer retention.
* **The Data:** 
  * Customers with No Internet Service: **7.14% loss rate**
  * Customers **With** Tech Support: **15.17% loss rate**
  * Customers **Without** Tech Support: **41.64% loss rate**
* **Key Business Insight:** Leaving customers to set up or troubleshoot technology on their own is a massive breaking point. Customers who do not have Tech Support are **nearly 3x more likely to leave** than those who do, pointing to frustration during product setup.

### Challenge 3: Service "Stickiness" & Bundling Power
* **The Goal:** Find out if selling multiple services to a single customer increases their long-term loyalty.
* **The Data:** 
  * 0 Extra Services: **475 customers lost** | 1 Extra Service: **442 lost** | 2 Extra Services: **370 lost**
  * 3 Extra Services: **306 lost** | 4 Extra Services: **190 lost** | 5 Extra Services: **71 lost** 
  * 6 Extra Services: **15 lost**
* **Key Business Insight:** There is a direct link between the number of services a customer buys and their loyalty. The sweet spot is exactly **4+ services**. Once a customer buys 4 or more services, customer loss drops drastically from hundreds down to double digits. 

### Challenge 4: High-Value Customer (HVC) Revenue Risk
* **The Goal:** Isolate top-tier clients and calculate the future revenue risk facing the business.
* **The Data:** **99 Premium Tier accounts** have left the company, wiping out **$598,711** in predicted future lifetime value.
* **Key Business Insight:** While losing 99 customers sounds small, their financial impact is massive. Losing a single premium customer causes significantly more financial damage to the bottom line than losing a standard customer.

### Challenge 5: Senior Citizen Demographics & Digital Exclusion
* **The Goal:** Examine whether digital-only updates (like online billing) cause frustration for older customers.
* **The Data:** 
  * Seniors using Traditional Paper Bills: **78 lost**
  * Seniors forced onto Paperless Digital Bills: **398 lost**
  * Non-Seniors with Paperless Bills: **1,002 lost** | Non-Seniors with Paper Bills: **391 lost**
* **Key Business Insight:** Forcing older customers to use digital-only billing causes major administrative friction. Seniors forced into paperless billing leave at **more than 5x the volume** of seniors using traditional paper invoices, showing clear demographic digital exclusion.

---

## 🚀 Strategic Solutions for All 5 Challenges

1. **Revenue Protection Plan (Challenge 1 Solution):** Shift 15% of the marketing acquisition budget into customer retention teams to actively halt the $2.86M historical revenue drain.
2. **Complimentary Tech Support Bundles (Challenge 2 Solution):** Include 3 months of free Tech Support with all new high-speed internet setups. This directly addresses the 41.64% customer loss rate by helping users during their critical onboarding phase.
3. **Ecosystem Product Discounts (Challenge 3 Solution):** Launch a targeted email/SMS campaign offering a discount to current customers who only hold 0–2 extra services. This systematically encourages them to upgrade to the highly loyal 4+ service bundle.
4. **"White-Glove" VIP Retention Squad (Challenge 4 Solution):** Form a dedicated customer service team to proactively reach out to and protect active clients in the top 10% lifetime value bracket, protecting up to $598,711 in future company value.
5. **Flexible Billing Access for Seniors (Challenge 5 Solution):** Adjust signup workflows to let customers aged 65+ easily choose traditional paper billing without paying extra fees. This completely removes the billing hurdle that cost the company 398 senior accounts.
