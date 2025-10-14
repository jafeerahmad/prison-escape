# Helicopter Prison Escape Analysis: Scripted Walkthrough

## 1. Introduction

This analysis explores the phenomenon of helicopter prison escapes using a dataset sourced from Wikipedia. The goal is to uncover patterns, trends, and insights into the frequency, geography, success rates, and notable individuals involved in these daring escapes.

---

## 2. Data Collection & Preparation

- **Source:** Wikipedia's "List of helicopter prison escapes" page
- **Data Format:** Tabular, 48 rows, 6 columns
- **Libraries Used:** requests, BeautifulSoup, pandas, matplotlib, numpy, re, unicodedata

**Script Steps:**
1. Download the web page using `requests`.
2. Parse HTML with `BeautifulSoup`.
3. Locate the relevant table and extract header/data rows.
4. Convert data to a pandas DataFrame.
5. Save the DataFrame to `prison.csv`.
6. Remove redundant columns (e.g., "Details").

---

## 3. Temporal Analysis

**Questions:**
- How many escapes occurred each year?
- Are there trends or patterns over time?
- Are certain months/days more likely for escapes?

**Script Steps:**
1. Convert 'Date' column to datetime.
2. Extract year, month, and day of week.
3. Group and count escapes by year, month, and day.
4. Visualize with bar charts.

**Findings:**
- Highest escape years: 1986, 2001, 2007, 2009, 1988
- December, Sunday, Monday, and Thursday are peak times

---

## 4. Geographical Analysis

**Question:**
- Which countries have the most helicopter prison escapes?

**Script Steps:**
1. Group by 'Country' and count escapes.
2. Sort and visualize top countries.

**Finding:**
- France leads in recorded helicopter prison escapes.

---

## 5. Success Analysis

**Question:**
- What is the overall success rate?

**Script Steps:**
1. Count 'Succeeded' values ('Yes'/'No').
2. Calculate percentages.
3. Visualize with bar chart.

**Insight:**
- Success rate reveals security strengths/weaknesses. Data may be incomplete due to underreporting.

---

## 6. Escapee Analysis

**Questions:**
- What is the average number of escapees per incident?
- Who are the most persistent escapees?

**Script Steps:**
1. Calculate average escapees per incident.
2. Identify individuals with multiple escape attempts.
3. Filter and display persistent escapees.

**Findings:**
- Average: ~1 escapee per incident
- Notable repeat escapees: Pascal Payet, Michel Vaujour, Vassilis Paleokostas

---

## 7. Case Studies: The Unstoppable Escapees

- **Vassilis Paleokostas (Greece):** Two helicopter escapes, remained at large for months.
- **Michel Vaujour (France):** Two escapes, one aided by his wife piloting a helicopter.
- **Pascal Payet (France):** Two escapes, led to reforms in French prison security.

---

## 8. Conclusion

This analysis revealed:
- Temporal and geographical patterns in helicopter prison escapes
- Success rates and their implications
- Stories of persistent escapees

**Limitations:**
- Data may be incomplete or biased
- Findings are subject to updates in the source

**Future Directions:**
- Further research into security measures
- Broader analysis of escape methods

---

