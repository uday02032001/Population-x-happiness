# Population-x-happiness

# 🌍 Power Query Project – World Population vs Happiness Index (2025)

> A pure Power Query challenge: No Excel formulas, no DAX, no SQL — just clean, merge, and analyze directly inside Power Query Editor.

## 📌 Project Overview

This project analyzes **global population data (2025)** alongside the **World Happiness Index (2024)**. The core challenge was to **extract, clean, transform, and analyze** the data using **only Power Query**, without relying on any other tools.

---

## 📂 Data Sources

- 🌐 **Population Dataset**: Scraped from [Worldometers](https://www.worldometers.info/world-population/population-by-country/)
- 📊 **Happiness Index Dataset**: Provided via Excel (2024 data only used)

---

## 🛠️ Power Query Techniques Used

- Web scraping using **Power Query's Web connector**
- Column value replacements (`"−"` to `"-"`, removing `%`, `,`)
- Manual country name standardization to align mismatched values (e.g., `Czechia` → `Czech Republic (Czechia)`)
- **Full outer joins** to identify unmatched countries
- **Custom columns** for:
  - Population projection (2026) using growth %
  - Country classification based on conditions
  - Range calculation (e.g., Median Age Range)
- Aggregations: **SUM, COUNT, AVERAGE**
- Filtering and sorting (Top N, Between, Greater Than/Less Than)
- Indexing for positional queries (e.g., 5th highest density)

---

## 📈 Key Questions Answered

- Top 3 countries by **population** and **happiness rank**
- Countries with population **decline** or **growth > 1%**
- Population **projection for 2026**
- Median age range of top 5 happiest countries
- Percentage of global population contributed by **India, Pakistan, and Bangladesh**
- Correlation: **Population size vs Happiness**
- Urbanization impact on happiness scores

---

## 📊 Insights Uncovered

- **India** has the world’s largest population but ranks **118th in happiness**
- **Smaller countries** tend to be happier than larger ones (avg 0.4 points higher happiness)
- Countries with **>50% urban population** are significantly happier on average (avg 6.0 vs 4.47)
- 62 countries are experiencing a **population decline**

