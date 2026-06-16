# 📱 OCA Indonesia: CPaaS Behavioral Architecture
> **Impact:** Engineered an adapted RFM framework to segment <mark><b>20 enterprise accounts</b></mark> and mitigate a 78% failure rate in Voice Call channels.

<p align="center">
  <a href="python_analysis.txt">
    <img src="https://img.shields.io/badge/View%20Python%20Code-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  </a>
  &nbsp;
  <a href="../assets/Revo Telco Segmentation.pdf" target="_blank">
    <img src="https://img.shields.io/badge/View%20Deck%20(PDF)-A68966?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" />
  </a>
</p>

## 📌 Project Summary
This project analyzes client behavior for OCA Indonesia, a Telkom Indonesia CPaaS platform. Previously, all enterprise users were treated uniformly. I implemented an adapted **RFM behavioral architecture** to drive user personalization, mitigate backend churn, and optimize infrastructure capacity across 5 core communication channels.

---

## 🚀 Achievements (AQS Framework)
* **Segmented** 20 enterprise CPaaS accounts using a custom rule-based RFM framework to identify high-value targets and churn risks.
* **Uncovered** a critical **~78% transaction failure rate** within the Voice Call channel, identifying a major backend infrastructure bottleneck.
* **Analyzed** 3 months of transaction data across 5 relational tables to extract distinct behavioral profiles and traffic patterns.
* **Formulated** data-driven routing strategies—specifically rerouting failed Voice requests to SMS/WhatsApp—to safeguard revenue pipelines.

---

## 📊 Visual Analysis & Technical Insights
*Key findings from the behavioral segmentation and channel performance audit.*

---

### 1. RFM Behavioral Architecture (The "Hero" Visual)
<table>
  <tr>
    <td width="60%">
      <img src="../assets/newplot (5).png.png" alt="RFM Scatter Plot" style="border-radius: 10px; border: 2px solid #A68966;">
    </td>
    <td valign="top">
      <h4>Key Insights:</h4>
      <ul>
        <li><b>Segmentation:</b> Categorized users into <b>Champions</b> (6 users/Rp 3M rev), <b>Loyal</b> (7 users), and <b>Low-Intensity</b> (7 users).</li>
        <li><b>Strategic Mapping:</b> The bubble size represents traffic frequency, highlighting the high-volume nature of our Champion cohort.</li>
      </ul>
    </td>
  </tr>
</table>

---

### 2. Channel Performance Audit (Text-Based Matrix)
*While the RFM analysis visualizes revenue, the infrastructure performance audit revealed stark channel disparities.*

| Channel | Status | Failure Rate | Recommendation |
| :--- | :--- | :--- | :--- |
| **WhatsApp/SMS** | Stable | Low | Standard Routing |
| **Voice Call** | **Unstable** | <mark><b>~78%</b></mark> | **Reroute to SMS/WA** |

> **Operational Insight:** High failure rates in Voice Call impact overall backend operational capacity. Rerouting failed peak-hour Voice requests to stable channels ensures Champions maintain service continuity.

---

### 3. Traffic Pattern & Revenue Strategy
* **For Champions:** Bundled discounts and priority traffic routing.
* **For Loyal Clients:** High-margin cross-sell campaigns.
* **For Low-Intensity:** Migrated to automated self-service developer playbooks to reduce support overhead.

---

## 🛠️ Tools & Methods
- **Python (Google Colab):** Rule-based RFM scoring, Percentile Ranking, Data Wrangling across 5 tables.
- **Methods:** RFM Architecture Mapping, Percentile Choice Ranking (used as an alternative to K-Means for small, distinct cohorts), Channel Traffic Pattern Analysis.

---
<p align="center">
  <a href="../projects.html"><b>← Back to Project Archive</b></a>
</p>

