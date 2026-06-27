# Red Bull In-Store Shopper Experience | Power BI Dashboard

A Power BI project analysing in-store shopper experience for Red Bull across Australian retail channels.
Built on a synthetic survey dataset of 630 respondents covering purchase behaviour, channel preferences,
satisfaction scores, shelf visibility and competitive switching triggers.

> **Disclaimer:** Synthetic dataset created for learning and portfolio purposes. Brand names are used for realism only and this project has no affiliation with Red Bull GmbH.

---

## Objective

To understand what drives Red Bull purchase decisions in-store, identify satisfaction gaps across key experience dimensions, and assess competitive switching risk across the Australian energy drink market.

---

## Tools Used

- **Power BI Desktop** - data cleaning, modelling and dashboard
- **Excel** - raw survey dataset

---

## Dataset Overview

| Detail | Info |
|---|---|
| Respondents | 630 |
| Survey Period | June 2024 - August 2024 |
| Geography | Australia (state-level) |
| Format | `.xlsx` |

---

## Data Cleaning Steps

## Data Cleaning Steps

All cleaning performed in **Power Query (Power BI Desktop).**

| Step | Column | Action |
|---|---|---|
| 1 | Purchase Channel | Split on `)` delimiter — freetext responses consolidated under `Other` |
| 2 | Red Bull Variant | Split on `:` delimiter — seasonal/limited editions grouped as `Other` |
| 3 | Price Per Can | Duplicated column → split digit to non-digit → replaced `-` and `+` → converted to whole number → averaged to single price estimate |
| 4 | Secondary Purchase Trigger | Column removed — analysis scoped to primary trigger only |
| 5 | Purchase Trigger | Split on `:` delimiter — freetext responses consolidated under `Other` |
| 6 | State / Region & Competitor Brands | Same delimiter split applied — freetext responses consolidated under `Other` |

## Dashboard

*(Screenshots and Power BI Service link — coming soon)*

---

## Key Insights

*(To be updated after dashboard is built)*
