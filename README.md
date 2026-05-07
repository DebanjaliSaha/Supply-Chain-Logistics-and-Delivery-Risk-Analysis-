# Supply Chain Delivery Performance Analysis

**End-to-end delivery performance and logistics analysis across 180k+ orders — uncovering a systemic 57.28% late delivery rate, a shocking 100% First Class failure, and $11.5M revenue at risk in Western Europe ($5.89M) and Central America ($5.67M)**
---

## ⚡ TL;DR — For Recruiters

> **57.28% of 180,519 orders are late** — a systemic supply chain failure affecting every region, every customer segment, and every product category.

| What I Found | Why It Matters |
|---|---|
| 🔴 First Class shipping: **100% late rate** | Customers paying premium price are always let down |
| 🔴 Second Class: **79.7% late, 1.99 days avg delay** | Mid-tier option is the worst by severity |
| 🟢 Standard Class: **39.8% late** | Cheapest mode outperforms all premium options |
| 🌍 Western Europe + Central America: **$11.5M revenue at risk** | Highest-volume regions with highest delay rates |
| 💰 Late vs On-Time profit gap: **only $0.25 (median)** | No customer compensation system exists |
| 📦 Golf Bags & Carts: **68.8% late** | Worst product category on both frequency and severity |
| 📊 Profit kurtosis: **71.38** | Profit averages are statistically unreliable — median tells the real story |

---

## 🎯 Business Problem

A global e-commerce supply chain is silently failing its customers. Despite operating across 23 regions and 4 shipping modes, **more than 1 in every 2 orders arrives late** — yet this crisis goes largely undetected because profit averages appear stable on the surface.

This analysis peels back that surface to identify *where* delays are happening, *which* shipping modes are broken, *which* regions carry the highest business risk, and *why* conventional profit metrics are masking the true operational damage.

---

## 💡 Critical Insights Discovered

### 🔥 1. System-Wide Delivery Failure *(Anchor Finding)*
> **57.28% of all 180,519 orders are delivered late** — meaning more than half of every customer interaction ends in a broken promise.

- Median delay = 1 full day, despite a mean of only 0.57 days — confirming the average understates the reality most customers face
- Delays are consistent across ALL regions (51–60%) and ALL customer segments (~57%), ruling out any isolated regional or demographic cause
- **This is not a regional problem. It is a systemic operational failure.**

---

### 🔥 2. Premium Shipping Paradox *(Most Shocking Finding)*
> **First Class shipping has a 100% late delivery rate.** Every single customer who pays premium price for First Class receives their order late — without exception.

| Shipping Mode | Late Rate | Avg Delay | Volume Share |
|---|---|---|---|
| First Class | 100.0% 🔴 | 1.00 day | 15.4% |
| Second Class | 79.7% 🔴 | 1.99 days | 19.5% |
| Same Day | 47.8% 🟡 | 0.48 days | 5.4% |
| Standard Class | 39.8% 🟢 | -0.004 days | 59.7% |

- Standard Class — the cheapest and most used mode (60% of all orders) — **outperforms all premium options**
- Second Class averages nearly **2 full days late**, the worst severity of any mode
- Customers paying more are consistently receiving worse service — a fundamental breakdown in operations

---

### 🔥 3. High-Impact Regional Risk *(Business Priority Finding)*
> **Western Europe and Central America combine the highest late rates with the two largest sales volumes** — making them the highest financial risk regions in the entire portfolio.

| Region | Late Rate | Total Sales | Risk Level |
|---|---|---|---|
| Western Europe | 58.5% | $5.89M 🔴 | Critical |
| Central America | 57.2% | $5.67M 🔴 | Critical |
| South Asia | 58.5% | $1.55M 🟡 | High |
| Canada | 51.9% | $0.19M 🟢 | Low |

- Improving delivery in Western Europe and Central America alone would impact **~30% of total order volume**
- Central Africa has the highest late rate (60.7%) but only $327K in sales — high frequency, low business priority
- Canada is the only region performing meaningfully below the 57% average

---

### 📊 4. Profit Outlier Crisis *(Statistical Warning)*
> **10.49% of all orders (18,942 records) are profit outliers**, with extreme values reaching as low as **-$4,275 per order**.

- IQR boundaries: -$79.70 (lower) to $151.50 (upper) — any profit outside this range is statistically extreme
- Order Profit Per Order shows **kurtosis of 71.38** (71x more extreme than normal distribution) and **skewness of -4.74**
- Median profit ($31.52) is **$9.55 higher than mean profit ($21.97)** — extreme loss transactions are actively understating true profitability
- All profit-based averages in this dataset should be interpreted using median, not mean

---

### 💰 5. Late Deliveries Don't Hurt Profit — And That's the Problem
> **Mean profit difference between late and on-time orders: only $0.91. Median difference: only $0.25.**

| Delivery Status | Mean Profit | Median Profit |
|---|---|---|
| On Time | $22.50 | $31.68 |
| Late | $21.59 | $31.43 |

- Both mean and median confirm the same finding — late deliveries have virtually zero financial impact on profit per order
- This strongly suggests **customers are not receiving refunds, compensation, or discounts** for late deliveries
- The business is absorbing the operational failure without financial consequences *yet* — but customer trust and long-term retention are at invisible risk

---

### 🚚 6. Shipping Mode Profit Sensitivity
> **Same Day shipping loses the most profit when late (-$4.48 per order)**, making it the most financially sensitive mode to delays.

| Shipping Mode | On-Time Profit | Late Profit | Difference |
|---|---|---|---|
| Same Day | $22.99 | $18.51 | -$4.48 🔴 |
| Second Class | $22.60 | $20.98 | -$1.62 |
| Standard Class | $22.45 | $21.32 | -$1.13 |
| First Class | N/A | $23.12 | N/A* |

*First Class has no on-time orders to compare against — 100% are late

---

### 📦 7. Category-Level Delay Severity
> **Golf Bags & Carts is the worst performing product category on both frequency (68.8% late) and severity (0.77 days average delay).**

- Top 5 worst categories by late rate: Golf Bags & Carts (68.8%), Lacrosse (62.1%), Cameras (62.0%), Pet Supplies (61.4%), Sporting Goods (59.9%)
- Best performing: Men's Golf Clubs (49.8%), Computers (52.7%), Golf Apparel (53.3%)
- Most categories cluster between 55–60%, again confirming systemic rather than category-specific delays

---

### 👥 8. Customer Segment Impact *(Ruling Out a Variable)*
> **All customer segments show near-identical late rates** — Consumer (57.3%), Corporate (57.1%), Home Office (57.5%).

- Delays are completely indifferent to customer type
- Corporate clients — typically highest value and hardest to replace — are experiencing the same failure rate as every other segment
- This rules out customer segmentation as a driver and reinforces the systemic conclusion

---

## 📊 Statistical Analysis Summary

| Analysis | Key Finding |
|---|---|
| Descriptive Statistics | Sales avg $203.77 (median $199.92), Profit avg $21.97 (median $31.52) |
| Skewness | Delay Days: 0.03 ✅ (reliable) \| Profit: -4.74 🚨 (highly distorted) |
| Kurtosis | Delay Days: -0.29 ✅ \| Profit: 71.38 🚨 (extreme outlier concentration) |
| Outlier Detection | 18,942 profit outliers (10.49%) via IQR method |
| Correlation | Delay Days has near-zero correlation with all variables (max: -0.005) |
| Mean vs Median | Profit mean ($21.97) vs median ($31.52) — $9.55 difference, understating true profitability |

Correlation Matrix (key finding): Delay Days shows near-zero correlation with Order Quantity (0.002), Discount (-0.0002), Sales (-0.004), and Profit (-0.005) — confirming delays are not driven by any single measurable order characteristic but by structural logistics failures.

---


## 📐 Delivery Risk Segmentation

Rather than treating all shipping modes and regions equally, this analysis segments them into performance tiers to enable **prioritized operational action**.

### Shipping Mode Risk Segmentation

| Shipping Mode | Late Rate | Risk Tier |
|---|---|---|
| First Class | 100.0% | 🔴 High Risk |
| Second Class | 79.7% | 🔴 High Risk |
| Same Day | 47.8% | 🟢 Low Risk |
| Standard Class | 39.8% | 🟢 Low Risk |

**Segmentation logic:** Critical High Risk (≥70%), Medium Risk (50-70%), Low Risk (<50%)

### Region Risk Segmentation

| Risk Tier | Regions | Late Rate Range |
|---|---|---|
| 🔴 High Risk | Western Europe, South Asia, Central Africa, South of USA, Southeast Asia, East of USA | ≥58% |
| 🟡 Medium Risk | West Asia, East Africa, Eastern Europe, Central America, South America, Central Asia, US Center, Eastern Asia, Southern Europe, North Africa, West of USA, Northern Europe, Southern Africa, Oceania, Caribbean | 55–58% |
| 🟢 Low Risk | West Africa, Canada | <55% |

**Priority action:** High Risk regions with high sales volume (Western Europe, Central America) should be addressed first.

### Product Category Risk Segmentation

Rather than listing all 50 categories, this analysis focuses on the **top 5 worst and top 5 best** performers to identify where product-specific logistics intervention is most needed.

**🔴 Top 5 Worst Categories (Highest Delay):**

| Rank | Category | Late Rate | Avg Delay Days |
|---|---|---|---|
| 1 | Golf Bags & Carts | 68.8% | 0.77 days |
| 2 | Lacrosse | 62.1% | 0.66 days |
| 3 | Cameras | 62.0% | 0.65 days |
| 4 | Pet Supplies | 61.4% | 0.71 days |
| 5 | Sporting Goods | 59.9% | 0.62 days |

**🟢 Top 5 Best Categories (Lowest Delay):**

| Rank | Category | Late Rate | Avg Delay Days |
|---|---|---|---|
| 1 | Men's Golf Clubs | 49.8% | 0.33 days |
| 2 | Computers | 52.7% | 0.45 days |
| 3 | Golf Apparel | 53.3% | 0.47 days |
| 4 | CDs | 54.2% | 0.46 days |
| 5 | Baby | 54.6% | 0.44 days |

**Segmentation logic:** High Risk (≥60% late), Medium Risk (55–60%), Low Risk (<55%)

**Key observation:** Golf Bags & Carts is the only category that ranks worst on BOTH metrics simultaneously — highest late rate (68.8%) AND one of the highest average delays (0.77 days). This dual-metric failure makes it the single highest priority category for supply chain intervention.

---

## 🔄 Workflow Architecture
```
Raw Dataset (53 columns, 180,519 rows)
↓
Data Cleaning & Preprocessing
(Dropped 22 columns · Fixed dtypes · Handled missing values)
↓
Feature Engineering
(Created Delay Days & Is Late columns)
↓
Exploratory Data Analysis
(Univariate → Bivariate → Multivariate)
↓
Statistical Analysis
(Outlier Detection · Skewness · Kurtosis · Correlation)
↓
Delivery Risk Segmentation
(Shipping Mode · Region · Product Category)
↓
Power BI Interactive Dashboard
↓
Business Insights & Recommendations
```

## 🛠️ Tools & Technologies

**Programming & Environment**
- Python 3
  - Pandas
  - NumPy

**Development Environment**
- Jupyter Notebook

**Business Intelligence**
  - Power BI
  - Interactive Dashboard
  - Data Modeling
  - KPI Reporting
  - Cross-filtering & Slicers

**Analysis Techniques**
- Data Cleaning & Feature Engineering
- Exploratory Data Analysis (EDA)
- Descriptive Statistical Analysis
- IQR Outlier Detection
- Skewness & Kurtosis Analysis
- Correlation Analysis
- Mean vs Median Comparison
- Delivery Risk Segmentation
- Business Insight Translation

## 📊 Power BI Dashboard

### Delivery Performance Overview
<img width="1291" height="769" alt="Screenshot (424)" src="https://github.com/user-attachments/assets/05bcf7b1-0d40-44a8-85cf-22478ec9704f" />

*Delivery performance overview across 180,519 orders — KPI cards, Late vs On-Time distribution, regional failure rates, and shipping mode performance.*

### Risk Segmentation & Profit Impact 
<img width="1265" height="698" alt="Screenshot (425)" src="https://github.com/user-attachments/assets/f2d5df31-1706-4e8a-897e-4fb5b403da20" />


*Risk segmentation and profit impact analysis — delay severity by category and shipping mode, regional risk table, and profit comparison by delivery status.*

## 💼 Business Impact & Recommendations

### Immediate Actions (0–30 days)
- **Halt First Class as currently operated** — 100% failure rate is unacceptable for a premium-priced service. Audit the entire First Class fulfillment pipeline before accepting new orders under this tier.
- **Investigate Second Class logistics** — 1.99 days average delay and 79.7% late rate indicate a broken fulfillment process, not random variance.

### Short-Term Actions (1–3 months)
- **Focus operational resources on Western Europe and Central America** — these two regions represent 30% of orders and the highest sales exposure. Even a 10% improvement in late rate would protect millions in revenue.
- **Redesign premium shipping SLAs** — if Standard Class consistently outperforms First Class and Second Class, the company's shipping tier logic needs a fundamental rebuild.

### Long-Term Actions (3–12 months)
- **Establish customer compensation policy for late deliveries** — current data shows near-zero profit impact from late orders, suggesting no compensation exists. This may protect short-term profit but erodes customer lifetime value silently.
- **Investigate Golf Bags & Carts supply chain** — highest delay category on both frequency and severity; likely a warehousing or supplier lead time issue.
- **Implement real-time delivery performance monitoring** — a 57% late rate at this scale suggests no early warning system currently exists.

---

## 📁 Repository Structure

```
├── README.md                              # Project documentation
├── supply_chain_delivery_analysis.ipynb   # Full Jupyter Notebook (cleaning + EDA + stats + segmentation)
├── DataCoSupplyChainDataset.csv           # Raw dataset (180,519 records)
```

---

## 🔮 Future Enhancements

- **Predictive Modeling**: Logistic regression or XGBoost to predict late delivery probability before shipment
- **Time-Series Analysis**: Identify seasonal delay patterns across months and quarters
- **Customer Impact Analysis**: Estimate long-term revenue risk from eroded customer trust due to repeated late deliveries
- **Root Cause Drill-Down**: Warehouse-level or carrier-level analysis to identify specific failure points within First Class and Second Class operations

---

## 🔗 Connect

**Author**: Debanjali Saha

📧 debanjalisaha508@gmail.com | 💼 [LinkedIn](https://www.linkedin.com/in/debanjalisaha510/) | 🐙 [GitHub](https://github.com/DebanjaliSaha)

---

*End-to-end supply chain delivery performance analysis | Python + Jupyter Notebook | 180,519 orders | 17 documented insights*

**Tags**: `#SupplyChain` `#DataAnalytics` `#Python` `#EDA` `#LogisticsAnalysis` `#DeliveryPerformance` `#Pandas` `#StatisticalAnalysis` `#PortfolioProject` `#DataScience`
