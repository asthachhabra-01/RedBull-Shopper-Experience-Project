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

- **Power BI Desktop** — data cleaning in Power Query, DAX measures, dashboard design
- **Excel** — raw survey dataset

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

All cleaning performed in **Power Query (Power BI Desktop).**

| Step | Column | Action |
|---|---|---|
| 1 | Purchase Channel | Split on `)` delimiter — freetext responses consolidated under `Other` |
| 2 | Red Bull Variant | Split on `:` delimiter — seasonal/limited editions grouped as `Other` |
| 3 | Price Per Can | Duplicated column → split digit to non-digit → replaced `-` with null and `+` with `7` → converted to whole number → averaged both columns to derive estimated price per can. Transformation completed but excluded from final dashboard visuals. |
| 4 | Secondary Purchase Trigger | Column removed — analysis scoped to primary trigger only |
| 5 | Purchase Trigger | Split on `:` delimiter → freetext responses consolidated under `Other` → labels shortened: `Eye-catching shelf placement` → `Shelf Placement`, `Recommended by someone` → `Word of Mouth` |
| 6 | State / Region & Competitor Brands | Same delimiter split applied — freetext responses consolidated under `Other` |
| 7 | Gender | `Non-binary / third gender` and `Prefer not to say` merged into `Other / Prefer Not to Say` using Replace Values |


---

## Key Insights

**1. Red Bull's product fundamentals are strong but value perception is a gap**
In-Store Availability (7.5) and Taste & Flavour (7.5) score highest across all satisfaction dimensions, confirming strong distribution and product quality. However Value for Money (5.7) and Promotions & Deals (5.4) are the two weakest scores — signalling a clear gap in perceived price fairness that represents an actionable opportunity for the commercial team.

**2. Brand Loyalty is the #1 purchase driver**
149 out of 480 shoppers cited Brand Loyalty as their primary purchase trigger, followed by Price / Promotion (138) and Shelf Placement (110). This confirms Red Bull's brand equity is doing significant heavy lifting in-store — but with Price / Promotion as a close second, promotional mechanics remain an important lever.

**3. Purchase is heavily impulse-driven among male shoppers**
Males are the dominant survey cohort and skew toward higher frequency purchasing — "Once a week" (96) and "Several times a week" (82) are the top two frequencies for male shoppers. Female shoppers show a similar pattern but at lower volumes, indexing more toward "Once a week" and "A few times a month."

**4. NSW and VIC represent the core shopper base**
NSW and VIC together account for the majority of survey respondents, consistent with population distribution across Australia. QLD and WA follow. This geographic concentration should inform where in-store activation and field sales resources are prioritised.

**5. Average shopper is 35 years old**
The average age of 35 sits at the upper end of Red Bull's traditional 18-34 target demographic — suggesting the brand has strong retention into the mid-30s age bracket, which has positive implications for lifetime value but may warrant a renewed focus on recruiting younger shoppers.
