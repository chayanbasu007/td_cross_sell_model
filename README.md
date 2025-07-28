### 📊 Bank Client Data — Column Descriptions

---

### 📝 Summary
- The data is related with direct marketing campaigns of a Portuguese banking institution.
- The marketing campaigns were based on phone calls.
- Often, more than one contact to the same client was required, in order to assess if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

### 🗓️ Campaign Duration
**May 2008 to November 2010**

### 💼 Client Demographics
- **age** *(numeric)*: Age of the client
- **job** *(categorical)*: "admin.", "unknown", "unemployed", "management", "housemaid", "entrepreneur", "student", "blue-collar", "self-employed", "retired", "technician", "services"
- **marital** *(categorical)*: "married", "divorced", "single"
- **education** *(categorical)*: "unknown", "secondary", "primary", "tertiary"
    1. **Primary** - basic.4y, basic.6y
    2. **Secondary** - basic.9y, high.school, professional.course
    3. **Tertiary** - university.degree
- **default** *(binary)*: "yes", "no"
- **balance** *(numeric)*: Average yearly balance (in euros)
- **housing** *(binary)*: "yes", "no"
- **loan** *(binary)*: "yes", "no"

### 📞 Contact Information
- **contact** *(categorical)*: "unknown", "telephone", "cellular"
- **day** *(numeric)*: Day of last contact
- **month** *(categorical)*: "jan", "feb", "mar", "apr", "may", "jun", "jul", "aug", "sep", "oct", "nov", "dec"
- **duration** *(numeric)*: Duration of last contact (in seconds)

### 🔁 Campaign Details
- **campaign** *(numeric)*: Number of contacts during this campaign
- **pdays** *(numeric)*: Days since last contact in a previous campaign
- **previous** *(numeric)*: Number of contacts before this campaign
- **poutcome** *(categorical)*: "unknown", "other", "failure", "success"

### 🎯 Target Variable
- **y** *(binary)*: "yes", "no"

---

## 📐 Data Shape
There are **45,211 rows** and **17 columns**.
- 16 feature columns
- 1 target column

---

## 👥 Job Profile Insights
- Majority of the people contacted are from Management, Technician, Blue-collar, Administrators, or Services.
- Together these groups comprise **80%** of the clients contacted during this marketing campaign.
    - 🔧 21.5% Blue-collar
    - 🧑‍💼 20.9% Management
    - 🛠️ 16.8% Technicians
    - 🗃️ 11.4% Administrators
    - 🛎️ 9.2% Services

---

## 💍 Marital Status Insights
- 👩‍❤️‍👨 60% of the clients were married
- ❤️ 28% are single
- 💔 12% are divorced

---

## 🎓 Education Insights
- Highest number of clients contacted have passed **secondary** level of education
- Second highest: **tertiary** level
- 15.2% clients contacted have passed **primary** level
- Education qualification of **4.1%** clients remains unknown

---

## 💳 Credit Default Insights
- Only **1.8%** clients contacted by the bank have a credit default history

---

## 🏠 Mortgage Insights
- 55.6% clients contacted by the bank have a **mortgage**
- 44.4% customers **don't have a mortgage**

---

## 💼 Personal Loan Insights
- Only **16%** of customers have a **personal loan**
- The rest do not

---

## 🏦 Loan Holding Insights
- 38.1% clients do **not hold any kind of loan**
- 61.9% clients hold **at least one kind of loan** (either HL or PL or both)
    - 6.4% hold only Personal Loans
    - 45.9% hold only Mortgages
    - 9.7% hold both Mortgage and Personal Loans

---

## ☎️ Contact Mode Insights
- 64.8% clients were contacted by **device**
- 6.4% clients were contacted by **telephone**
- Mode of contact remains **unknown** for 28.8% clients

---

## 🗓️ Month Insights
Majority of the clients were contacted in mid-year:
- 🌸 30.4% in May
- ☀️ 15.3% in July
- 🌻 13.8% in August
- 🌦️ 11.8% in June
- 🍂 8.8% in November
- ❄️ Lowest in December (~0.5%)

---

## 🕒 Quarter Insights
- 48.7% clients were contacted in **Q2**
- 30.3% in **Q3**
- Only 20% in **Q1** and **Q4** (beginning and end of year)
- Together, Q2 and Q3 comprise ~80% of the overall clients contacted

---

## 🎯 Conversion Breakdown
- ✅ **Converted**: 11.7%
- ❌ **Not Converted**: 88.3%

> Clients who converted from the campaign are significantly outnumbered by those who didn’t.

---

## 🔍 Key Insights

### ⚠️ High Drop-off Rate
- A staggering **88.3%** of clients chose not to convert
- Highlights a critical **bottleneck** in the campaign funnel—either in targeting, messaging, or offer attractiveness

### 🌱 Growth Opportunity
- Even though conversion is low, the **11.7%** who did convert present a **valuable engaged segment**
- Understanding what worked for this group could help replicate success elsewhere

### 📉 Effectiveness Concerns
- The current strategy may lack resonance with most clients
- It could be underperforming due to unclear value propositions or **misaligned targeting**

### 📌 Final Thought
The campaign’s low conversion rate isn’t a failure—it’s a **signal**

---

## 🧩 Campaign Performance Insights across Demographics

### 📌 Problem Statement
Analyze client conversion behavior across key demographics to refine future campaign targeting, enhance response rates, and prioritize segments with high engagement potential.

---

### 📊 Conversion Analysis Summary
Grouped bar charts across six dimensions—job, marital status, education, default history, housing loan status, and personal loan status. Each chart shows the percentage of clients who did **not convert** (red) versus those who **converted** (green).

---

### 👷 Conversion by Job Type
| Job Category   | Converted % | Key Insight |
|----------------|-------------|-------------|
| Management     | 2.9%        | 📋 Strong potential in higher-income groups. |
| Retired        | 1.4%        | 🧓 Opportunity in pensioners and financial security. |
| Technician     | 1.9%        | 🛠️ Good traction from skilled professionals. |
| Blue-collar    | 1.6%        | 🔧 Engaged despite economic constraints. |
| Student        | 0.1%        | 🎓 Very low uptake—targeting may not be viable. |

> 🛎️ **Focus on job types with economic stability and past success indicators.**

---

### 💍 Conversion by Marital Status
| Status  | Converted % | Insight |
|---------|--------------|---------|
| Married | 6.1%        | 👨‍👩‍👧‍👦 Most conversions, but also highest client base. |
| Single  | 4.2%        | ❤️ Higher relative engagement rate. |
| Divorced| 1.4%        | 💔 Low conversion—requires different messaging.

> ✨ **Target singles for higher response likelihood.**

---

### 🎓 Conversion by Education
| Education Level | Converted % | Insight |
|------------------|-------------|---------|
| Secondary        | 5.4%        | 📘 Most effective—likely practical decision-makers. |
| Tertiary         | 4.4%        | 🧠 Slightly lower—may need value-focused messaging. |
| Primary          | 1.3%        | 📗 Low conversions—less financial agility.

> 📚 **Align messaging style to education tiers.**

---

### 💳 Conversion by Default History
| Default Status | Converted % | Insight |
|----------------|-------------|---------|
| No             | 11.6%       | ✅ Default-free clients are significantly more receptive. |
| Yes            | 0.1%        | 🚫 Almost no conversions—credit risk barrier.

> ⚠️ **Consider excluding or segmenting defaulted clients.**

---

### 🏠 Conversion by Housing Loan
| Housing Loan | Converted % | Insight |
|--------------|-------------|---------|
| No           | 7.4%        | 🔓 More financially flexible, better conversion. |
| Yes          | 4.3%        | 🔒 Lower engagement—likely tied to obligations.

> 🏡 **Target non-loan clients for higher campaign ROI.**

---

### 💼 Conversion by Personal Loan
| Personal Loan | Converted % | Insight |
|----------------|-------------|--------|
| No             | 10.6%       | 🟢 Responsive—less financial strain. |
| Yes            | 1.1%        | 🔴 Minimal conversion—likely burdened.

> 💰 **Loan status is a strong predictor of campaign response.**

---

### ☎️ Conversion by Contact Method
| Contact Type | Converted % | Key Insight |
|--------------|--------------|--------------|
| Cellular     | 9.7%         | 📱 Highest engagement—mobile outreach is most effective. |
| Telephone    | 0.9%         | ☎️ Low conversions—traditional calls less impactful. |
| Unknown      | 1.2%         | ❓ High "No" responses—data may be unreliable or misclassified. |

> 🔍 **Recommendation**: Prioritize cellular outreach and audit "unknown" contact metadata.

---

### 📅 Conversion by Month
| Month     | Converted % | Key Insight |
|-----------|-------------|--------------|
| March     | 1.3%        | 🌱 Solid start to campaign season—good traction. |
| April     | 0.7%        | 🌤️ Moderate conversions—worth considering for mid-quarter push. |
| May       | High Volume, Low Rate | ⚠️ Popular month, but low yield. |
| August    | 1.5%        | ☀️ Highest conversion—peak month for targeting. |
| November  | Minimal     | ❄️ End-of-year fatigue—poor responsiveness. |
| December  | Minimal     | 🎄 Holiday slump—avoid campaigns. |

> 🗓️ **Recommendation**: Focus on Q2 and August for optimal engagement.

---

### 🔄 Conversion by Previous Outcome
| Outcome   | Converted % | Key Insight |
|-----------|-------------|--------------|
| Success   | 2.2%        | ✅ Strong predictor of future conversions. |
| Unknown   | 7.5%        | 🤷 Mixed outcomes—opportunity in ambiguity. |
| Failure   | Low         | 🔴 Poor conversions—requires better targeting. |

> 💡 **Recommendation**: Retarget based on prior campaign success and investigate unknowns.

---

### 🕒 Conversion by Quarter
| Quarter | Converted % | Key Insight |
|---------|-------------|--------------|
| Q1      | 1.8%        | 🌅 Modest engagement—warm-up phase. |
| Q2      | 4.5%        | 🌞 Peak performance—launch major campaigns here. |
| Q3      | 3.5%        | 🍂 Good follow-through—sustain momentum. |
| Q4      | 1.8%        | ❄️ Low response—budget fatigue and distractions.

> 📆 **Recommendation**: Align high-investment campaigns with Q2 and Q3 cycles.

---

### 🎯 Strategic Recommendations
- 🧠 Segment by **default status**, **loan history**, and **job type** to focus on conversion-ready groups.
- 🗣️ Personalize outreach for **singles** and **secondary-educated** clients.
- 🔍 Reframe messaging for high-potential segments like management and technicians.
- 🧪 Consider score-based targeting to exclude financially restricted profiles.
- 📆 Align high-investment campaigns with Q2 and Q3 cycles.
