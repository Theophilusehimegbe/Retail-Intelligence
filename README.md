<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3d4f2e,50:6b7c45,100:8a9e5a&height=220&section=header&text=Retail%20Intelligence&fontSize=62&fontColor=f5f0e8&fontAlignY=38&desc=Customer%20Analytics%20%7C%20Power%20BI&descSize=22&descAlignY=58&descColor=d4cbb8&animation=fadeIn" width="100%"/>

<br/>

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Records](https://img.shields.io/badge/Records-392%2C431-3d4f2e?style=for-the-badge)
![Dashboards](https://img.shields.io/badge/Dashboards-3-6b7c45?style=for-the-badge)


<br/>

*A Power BI analytics project exploring customer behaviour, loyalty and churn across 392,431 retail transactions through three interconnected dashboards: Store Performance, RFM Segmentation and Churn Analysis.*

<br/>

[![View Dashboard](https://img.shields.io/badge/View%20Interactive%20Dashboard-3d4f2e?style=for-the-badge)](https://app.powerbi.com/view?r=eyJrIjoiZTE2NWI0MDMtNzE1ZS00NTY0LWIyNzMtZmM4MDFhYzIwNDM4IiwidCI6IjE5NDVhZTU1LTc4YTAtNDUyMC05MjY0LTAwZDJkNjBhYTQyOCJ9)


<br/>

</div>

---

## Table of Contents

- [Project Background](#project-background)
- [Data Structure and Initial Checks](#data-structure-and-initial-checks)
- [Repository Structure](#repository-structure)
- [Executive Summary](#executive-summary)
- [Dashboard 1: Revenue and Sales Analysis](#dashboard-1-revenue-and-sales-analysis)
  - [Monthly Performance Breakdown](#monthly-performance-breakdown)
  - [Takeaways](#takeaways)
  - [Recommendations](#recommendations)
- [Dashboard 2: Customer Segmentation (RFM Analysis)](#dashboard-2-customer-segmentation-rfm-analysis)
  - [Recommendations](#recommendations-1)
- [Dashboard 3: Churn Analysis](#dashboard-3-churn-analysis)
  - [Recommendations](#recommendations-2)
- [Project Closing Remark](#project-closing-remark)
- [Links](#links)

---

## Project Background

In today's highly competitive retail landscape, growth is no longer driven solely by acquiring new customers. Instead, long-term success depends on a company's ability to understand customer behaviours, strengthen loyalty and prevent churn. This project was initiated to provide a comprehensive performance assessment of the retail store using advanced customer analytics.

The analysis was structured around three major pillars:

> **Store Performance (Revenue and Sales Analysis):** Assess overall revenue growth, customer contribution and high-value segments.

> **Customer Segmentation (RFM Analysis):** Classify customers based on recency, frequency and monetary value, identifying groups such as Champions, Loyal Customers, New Customers and At-Risk Customers.

> **Churn Analysis:** Investigate retention trends, churn patterns, regional and product-specific drivers of drop-off and opportunities to strengthen customer loyalty.

By connecting these pillars, the project identifies what drives growth, where value is concentrated and why customers leave, ultimately providing the business with actionable strategies to build sustainable, loyalty-driven growth.

---

## Data Structure and Initial Checks

The dataset was obtained from the store's transactional and customer management system. It contains a total of **392,431 records**, capturing both sales performance and customer behaviour across different regions and time periods.

| Table | Key Fields |
|---|---|
| Sales Data | Customer ID, Country, Product Description, Invoice Date, Quantity, Unit Price, Stock Code, Invoice No |
| Temporal Data | Year, Quarter, Month of transaction |
| RFM Metrics (Calculated) | Recency (days since last purchase), Frequency (total transactions), Monetary (total spend per customer) |
| Churn Metrics (Calculated) | Customer Type, Days Since Last Purchase, Last Purchase Date, Customer ID |

### Data Model

![Data Model](assets/data_model.png)

Prior to analysis, a series of data quality checks were conducted using **Power Query Editor** to ensure completeness, accuracy and reliability of insights:

- Handling missing values in customer demographics and product categories
- Checking for and removing duplicate transactions
- Standardising date formats to enable time-series analysis
- Ensuring consistency in region and product naming conventions

After these initial checks, the cleaned dataset was loaded into Power BI where three dashboards were developed. This structured approach ensured that the insights derived from the dashboards were accurate, reliable and actionable.

---

## Repository Structure

```
retail-intelligence/
│
├── README.md
├── Retail_Intelligence.pbix      ← Power BI report file
└── assets/
    ├── data_model.png            ← Data model and relationship view
    ├── store_performance.png     ← Revenue and Sales dashboard
    ├── rfm_segmentation.png      ← RFM Segmentation dashboard
    └── churn_analysis.png        ← Churn Analysis dashboard
```

---

## Executive Summary

> *The story of this business is one of impressive short-term success coupled with looming long-term risk.*

Over the last year, the store achieved record-breaking revenue of **£8.88M**, a staggering **+1,457% increase year-on-year**, driven by a surge in over 4,300 active customers. On the surface, these results signal rapid growth and strong market traction. But beneath this success lies a critical challenge: sustaining loyalty in a customer base that is increasingly fragile and unevenly distributed.

<br/>

<div align="center">

| Metric | Value |
|:---:|:---:|
| Total Revenue | £8.88M |
| YoY Growth | +1,457% |
| Active Customers | 4,300+ |
| Total Sales | 19K |
| Units Sold | 5M |
| Avg Order Value | £479.55 |
| Retention Rate | 59% |
| Churn Rate | 41% |

</div>

<br/>

**The Growth Engine: Champions Drive, But a Fragile Base Lies Beneath**

Nearly £5.2M in revenue comes from Champions, the top 22% of customers who are loyal, engaged and high-spending. But here lies the risk: a 10% decline in Champion spend equals a **£520K revenue loss**, a hit that would take months of new customer acquisition to recover from. Meanwhile, 34% of the base are new customers with a **0% retention rate**, meaning acquisition investments are not translating into long-term value.

**The Churn Problem: A Leak in the Bucket**

While 59% of customers are retained, the flip side is a **41% churn rate**. New and seasonal shoppers are not sticking around and post-peak drop-offs after the holiday season expose the weakness in customer engagement strategies. Every churned customer represents not just lost revenue but also a lost opportunity for referrals, reviews and long-term loyalty.

**The Bigger Picture: Growth That Must Be Guarded**

The store has mastered acquisition and short-term sales spikes. But it is leaking long-term value through churn and uneven engagement. Growth is real but fragile, too dependent on a small elite group of customers. By converting new and seasonal buyers into loyalists, the business could unlock exponential growth without needing to acquire at the same aggressive pace.

---

## Dashboard 1: Revenue and Sales Analysis

![Revenue and Sales Dashboard](assets/store_performance.png)

The store delivered £8.88M in revenue from 19K sales and 5M units across 4K customers, a remarkable **+1,457% growth** vs. last year. Customer acquisition surged, but the average order value rose only slightly (£479.55, +1.7% QoQ), showing that while volume is booming, spend per customer is not keeping pace.

### Monthly Performance Breakdown

**January to March**

Early months saw steady but moderate revenue, averaging below £300K monthly. Growth was present but not remarkable, with customer acquisition still scaling. Product sales were scattered, with mid-tier items like Hanging Heart T-Light Holders and Postage Party Bunting contributing steadily but not dominating.

**April to August**

Sales began to climb, reflecting seasonal demand buildup. By mid-year, growth accelerated, with product leaders like Paper Craft Little Birdie and Regency Candlestick 3 Tier emerging as clear top performers. Units sold crossed the multi-million mark, while new customer onboarding kept pace, reaching approximately 3.2K by August.

**September to December**

The story of the year is written in Q4. Revenue surged sharply, peaking near December, with monthly revenue almost tripling compared to early months. Customers spent more frequently, pushing average order size to 278.75 units per sale (+25.6% YoY). However, average order value grew only marginally, suggesting buyers are increasing volume, not price-point.

**Customer Concentration**

Analysis shows that a handful of top customers (e.g. ID 14911: £194K revenue) generated significantly more than the median. Growth is leaning heavily on a small number of buyers, creating both loyalty and dependency.

**Geographic Distribution**

Revenue was dominated by the UK, Europe and North America, while Asia and Africa showed early but promising activity. Expansion into emerging regions could spread growth more evenly.

### Takeaways

The store is scaling aggressively, but growth is concentrated in Q4, in a handful of products and among a small pool of top customers. While this has delivered record-breaking revenue, it also exposes the business to seasonal risk and customer churn risk.

### Recommendations

**Product Diversification**

Paper Craft Little Birdie (£184K) and Regency Candlestick 3 Tier (£124K) together make up a large slice of total revenue. If either line dips, overall sales could fall sharply.

- Increase visibility and marketing around mid-range products like Hanging Heart T-Light Holder (£82K) and Postage Party Bunting (£76K) to broaden revenue contribution
- Audit products contributing less than £5K annually and phase out or bundle them into promotions to clear inventory

> **Expected Outcome:** Reduce revenue dependency on top 2 products from ~35% to below 25% of total store revenue

**Customer Base Expansion**

The top 3 customers (IDs 14911: £194K, 12471: £123K, 14606: £117K) together contributed nearly £435K, or ~5% of revenue.

- Launch a tiered loyalty programme rewarding mid-tier customers (~£20K to £50K spend) with discounts or early access
- Identify one-time buyers and target them with win-back campaigns to convert them into repeat customers

> **Expected Outcome:** Reduce top 3 customer revenue concentration from 5% to 3% while lifting mid-tier contributions by +10%

**Seasonal Preparedness**

Q4 (October to December) accounts for the largest sales spikes, with December nearly tripling early-month performance.

- Build inventory buffers of top-selling items by September to prevent stockouts
- Launch targeted holiday campaigns in October, not just November and December, to spread demand and smooth operations

> **Expected Outcome:** Reduce order backlog by 15% in December and lift total holiday revenue by +12%

**Geographic Growth**

Asia and Africa together represent less than 10% of revenue despite growing signals.

- Run geo-targeted promotions offering free shipping thresholds for orders above £200
- Test localised bundles such as cultural gift sets or festival-specific items tailored to regional tastes

> **Expected Outcome:** Lift Asia/Africa revenue share from below 10% to 15% within the next fiscal year

---

## Dashboard 2: Customer Segmentation (RFM Analysis)

![RFM Segmentation Dashboard](assets/rfm_segmentation.png)

While revenue tells us what was earned, segmentation reveals where it came from. This analysis uses the **RFM (Recency, Frequency, Monetary)** model to segment customers into actionable categories, helping tailor strategies for growth, retention and reactivation.

<br/>

<div align="center">

| Segment | Revenue | Share | Retention |
|:---:|:---:|:---:|:---:|
| Champions | £5.2M | ~59% | 96% |
| Loyal Customers | £1.6M | 18% | 72% |
| New Customers | £1.1M | 12% | 0% |
| At-Risk Customers | £0.6M | 7% | — |
| Potential Loyalists | £0.3M | 4% | 92% |

</div>

<br/>

**Champions are the lifeblood of the business, but they carry too much weight**

Champions alone drive £5.2M, nearly 60% of total revenue. A 10% decline in Champion spend equals a **£520K loss**. The business is heavily reliant on this narrow segment, making Champions both the biggest strength and the greatest vulnerability.

**Loyal Customers are the rising stars, the next generation of Champions**

Loyal Customers contributed £1.6M in revenue. With the right loyalty incentives, they can graduate into Champions. Moving just 25% of Loyal Customers up the ladder could unlock an extra **£400K in revenue**.

**New Customers are plentiful but risk falling into churn**

At 34% of the customer base, New Customers generated £1.1M in revenue, proving acquisition campaigns are working. But first-time buyers are fragile. Without the right nudges, they often do not return. The story here is activation — transforming one-time shoppers into repeat buyers before they vanish into the At-Risk pool.

**At-Risk Customers represent silent leakage**

The £0.6M in at-risk revenue is a slow leak in a bucket. If ignored, that 7% could snowball into a much larger churn problem. Every lost At-Risk customer is a wasted acquisition and loyalty effort.

**Potential Loyalists are small but big in promise**

Currently £0.3M of revenue comes from Potential Loyalists. With nurturing, they can grow into Loyal Customers and even Champions, helping balance the over-reliance on the current Champion base.

### Recommendations

**Protect the Champions**

- Launch exclusive benefits: VIP previews, priority service, free shipping thresholds
- Build a feedback loop through quarterly surveys or early access groups
- Set up retention tracking alerts for declining order frequency among Champions

> Losing even 5% of Champions would hurt more than failing to acquire hundreds of new customers

**Elevate Loyal Customers into Champions**

- Offer tiered loyalty perks: double points weekends and spend thresholds that unlock Champion-style benefits
- Use personalised cross-sell campaigns to encourage higher average order values

> **Expected Outcome:** If 1 in 4 Loyal Customers becomes a Champion, this unlocks **£400K in incremental revenue**

**Activate New Customers before they slip away**

- Design a welcome journey: discounts on the second purchase and curated starter bundles based on first purchase
- Use trigger-based reminders: if a New Customer has not returned within 30 days, send a tailored offer

> **Expected Outcome:** Increase repeat purchase rate among New Customers by 15%, translating into **£165K more annual revenue**

**Rescue At-Risk Customers**

- Deploy win-back campaigns: time-sensitive discounts, "we miss you" emails, or surprise offers
- Offer a last-chance incentive: loyalty points expiry reminders or reactivation coupons

> **Expected Outcome:** Even recovering 30% of the £0.6M saves **£180K without any new acquisition spend**

**Cultivate Potential Loyalists**

- Encourage repeat behaviour with "buy twice, get a perk" style campaigns
- Track conversion into Loyal Customers with a target of 20% uplift in 12 months

> **Expected Outcome:** Converting just 20% of this group could add **£60K to £70K in incremental revenue**

---

## Dashboard 3: Churn Analysis

![Churn Analysis Dashboard](assets/churn_analysis.png)

This analysis explores customer churn dynamics, identifying how many customers were retained versus lost, which groups are most at risk and what patterns drive churn across time, product categories and regions.

<br/>

<div align="center">

| Metric | Value |
|:---:|:---:|
| Total Customers | 4,334 |
| Retained | 2,554 (59%) |
| Churned | 1,780 (41%) |
| YoY Retention Growth | +338% |
| YoY Churn Change | +10.5% worse |
| Champion Retention | 96% |
| Potential Loyalist Retention | 92% |
| Loyal Customer Retention | 72% |
| New Customer Retention | 0% |

</div>

<br/>

**The Retention and Churn Tug of War**

2,554 customers were retained, a 338% increase vs. last year. However, 1,780 customers churned, translating into a **41% churn rate**, which is 10.5% worse than last year. This reveals a paradox: while more customers are staying than before, an equally large pool is leaking out. Growth is unstable — if acquisition slows, churn will erase the gains.

**Customer Segment Loyalty Divide**

Champions (96% retention) and Potential Loyalists (92% retention) are the backbone of the business. Loyal Customers (72% retention) are showing cracks — nearly 3 out of 10 are slipping away. The real red flag is New Customers: **almost all of them churn after their first purchase (0% retention)**.

**Seasonal Churn Spikes**

September and December stand out as danger months. In December, churn peaks at its highest. Ironically, this is also when customer numbers spike, but these new buyers do not return in January. The store is excellent at attracting one-time seasonal buyers but struggles to convert them into loyal, repeat customers.

**Product Segments Tell Two Stories**

High-volume products drive strong retention (67%). Best sellers have the worst outcome **(31% retention)**. Customers buy them once but rarely return, suggesting they are often impulse buys or seasonal/gift-driven products. Revenue drivers are not always loyalty drivers.

**Regional Retention Imbalance**

The UK and Western Europe are solid performers. But in regions like Africa and Asia, customers make initial purchases and then vanish, suggesting a lack of localised engagement.

### Recommendations

**Rebuild the Onboarding Journey**

Right now, new customers are guaranteed to churn after their first order. This is the single biggest churn driver.

- Implement a structured welcome programme: thank-you emails, personalised product recommendations and discount codes for second purchases
- Trigger an early engagement campaign within the first 7 days after purchase

> Even if only 20% of new customers make a second purchase, it would significantly lift the retention curve and create a larger pipeline of future Champions

**Turn Seasonal Shoppers into Year-Round Buyers**

- Launch a "From Holiday to Everyday" campaign in January, offering vouchers or personalised bundles
- Create holiday bundles that tie into subscriptions so holiday buyers roll over into repeat customers

> Converting just 10 to 15% of holiday-only buyers could generate hundreds of repeat customers in Q1

**Strengthen the Middle (Loyal Customers at Risk)**

- Introduce a tiered loyalty programme with free shipping after 3 orders, early access to new products or exclusive discounts
- Personalise offers based on past purchases to make customers feel seen and valued

> Improving this group's retention by just 10% could double the pipeline of Champions

**Redesign Product Retention Strategy**

- Pair best sellers with high-volume products in bundled offers, converting one-off gift buyers into everyday shoppers
- Analyse which best sellers attract churn-heavy customers and retarget them with complementary products

> If best seller retention rises from 31% to 45%, the store could stabilise revenue and reduce dependency on acquisition

**Localise Retention in Emerging Regions**

- Offer region-specific promotions such as festival discounts and local bundles
- Optimise delivery and post-purchase support in Africa and Asia, as logistics challenges may drive churn

> A 10 to 15% lift in regional retention could unlock new growth markets and reduce dependence on Western Europe

---

## Project Closing Remark

> *This analysis reveals a business at a crossroads. The store has successfully built a core of fiercely loyal customers who love the brand, proving that the value proposition is strong. The challenge and opportunity lie in extending that successful experience to every new customer who walks through the door. By acting decisively on these recommendations, the business can plug the leaks in its customer base, transform one-time sales into lifelong relationships, and build a foundation for growth that is not just impressive, but enduring. The goal is clear: stop acquiring customers only to lose them and start building a business where every new customer becomes a future Champion.*

---

## Links

| Resource | Link |
|---|---|
| Interactive Power BI Dashboard | [View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZTE2NWI0MDMtNzE1ZS00NTY0LWIyNzMtZmM4MDFhYzIwNDM4IiwidCI6IjE5NDVhZTU1LTc4YTAtNDUyMC05MjY0LTAwZDJkNjBhYTQyOCJ9) |


---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8a9e5a,50:6b7c45,100:3d4f2e&height=140&section=footer&animation=fadeIn" width="100%"/>

</div>
