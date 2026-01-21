
# 📊 Publisher Inventory Yield & Revenue Optimization

## 📌 Problem Overview

Digital publishers rely heavily on advertising revenue, but **not all ad inventory performs equally**.
Despite high traffic volumes, many publishers face challenges such as:

* High impressions but **low revenue yield**
* Inefficient monetization across **devices, ad formats, and placements**
* Lack of visibility into **which inventory segments underperform**
* Difficulty prioritizing **optimization efforts with maximum revenue impact**

Without a structured analytical approach, teams risk focusing on the wrong segments and missing clear monetization opportunities.

### ❓ Why this analysis was needed

The core business problem was to:

* Identify **low-yield inventory segments**
* Understand **where revenue leakage is occurring**
* Provide **data-driven recommendations** to improve monetization efficiency without harming user engagement

This project addresses that gap by combining KPI analysis, segmentation, and yield-gap–based prioritization.

---

## 🗂 Dataset Description

The dataset represents ad performance data captured at a granular level across time, content, and inventory dimensions.

### 📄 Columns & Description

| Column Name         | Description                                                   |
| ------------------- | ------------------------------------------------------------- |
| `date`              | Timestamp of ad activity                                      |
| `page_type`         | Type of page where the ad was shown (Home, Article, Category) |
| `publisher_section` | Content category (Tech, Entertainment, Sports, News)          |
| `device`            | User device type (Mobile, Desktop)                            |
| `geography`         | User location (India, US, EU)                                 |
| `ad_slot`           | Placement of the ad on the page (Top, Mid, Bottom)            |
| `ad_format`         | Ad format type (Banner, Native, Video)                        |
| `impressions`       | Number of times the ad was displayed                          |
| `clicks`            | Number of ad clicks                                           |
| `revenue`           | Revenue generated from the ad impressions                     |

---

## 🧮 Data Processing & Analysis

The following analytical steps were performed using **Python (Pandas)** and **Power BI (DAX)**:

### 🔹 KPI Calculations

* Click Through Rate (CTR)
* Revenue per Mille (RPM)
* Effective Cost per Mille (eCPM)
* Segment-level RPM
* Yield Gap (Segment RPM − Overall RPM)

### 🔹 Exploratory Data Analysis (EDA)

* Performance comparison across:

  * Devices
  * Ad formats
  * Ad slots
  * Publisher sections
* Identification of high-traffic but low-revenue segments
* Baseline benchmarking using overall platform metrics

### 🔹 Segmentation & Yield Gap Analysis

* Inventory segmented by:

  * Page type
  * Device
  * Ad slot
  * Ad format
* Yield gaps computed to identify underperforming inventory
* High-impression, low-RPM segments prioritized for optimization

---

## 📊 Power BI Report

The analysis is presented through a **2-page Power BI dashboard**, designed for executive clarity and actionable insights.

---

## 📄 Page 1: Inventory Yield & Revenue Overview

### 🎯 Purpose

Provide a **high-level performance snapshot** and highlight key monetization trade-offs.

### 🔍 Visuals Included

* **KPI Cards**

  * Total Impressions
  * Total Revenue
  * Overall CTR
  * Overall RPM
  * Overall eCPM

* **Ad Format Performance**

  * Comparison of RPM across Banner, Native, and Video formats

* **Publisher Section Performance**

  * Revenue efficiency across Tech, Entertainment, Sports, and News

* **Device Performance Overview**

  * RPM and engagement comparison between Mobile and Desktop

* **Revenue vs Impressions Scatter Plot**

  * Identifies high-traffic vs high-yield segments

* **Contextual KPIs**

  * % of Low-Yield Inventory
  * Lowest RPM Segment Indicator

### 🔑 Key Insights from Page 1

* Mobile drives higher engagement, but Desktop delivers higher revenue efficiency
* Video ads significantly outperform Banner ads in RPM
* Tech and Entertainment sections attract premium monetization
* A large share of impressions comes from underperforming inventory

---

## 📄 Page 2: Low-Yield Inventory – Optimization Deep Dive

### 🎯 Purpose

Identify **where to act first** by diagnosing low-yield inventory at a granular level.

### 🔍 Visuals Included

* **Low-Yield Inventory Table**

  * Page Type
  * Device
  * Ad Slot
  * Ad Format
  * Impressions
  * Segment RPM
  * Overall RPM (Benchmark)
  * Yield Gap (with conditional formatting)

* **Yield Gap by Ad Format**

  * Highlights formats contributing most to revenue leakage

* **Slot × Format RPM Matrix**

  * Reveals placement-level inefficiencies

### 🔑 Key Insights from Page 2

* Mobile Banner inventory consistently underperforms across page types
* High-impression segments often monetize below the platform average
* Video formats generate positive yield gaps across most placements
* Yield Gap analysis helps prioritize optimization efforts with maximum impact

---

## 🚀 Outcome & Business Impact

This project enables stakeholders to:

* Clearly identify **low-yield inventory**
* Focus optimization on **high-impact segments**
* Improve monetization efficiency through **data-driven decisions**
* Design controlled **A/B tests** for validating optimization strategies

---

## 🛠 Tools & Technologies Used

* **Python:** Pandas, NumPy
* **Power BI:** DAX, Interactive Dashboards
* **SQL concepts:** Aggregation, segmentation logic
* **Analytics Techniques:** KPI analysis, yield gap analysis, monetization optimization

---

## 📌 Final Note

This project demonstrates a **Product Analyst approach** — moving from data to insights, from insights to actions, and from actions to measurable impact.

