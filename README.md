# Seasonal-Funnel-Analysis-for-an-E-Commerce-Business

## 📌 Objective
To perform an end-to-end funnel analysis of a high-traffic retail dataset (GA4) during the Q4 sales peak, identifying how seasonal events — Black Friday, Cyber Monday, and Christmas —distort conversion behaviour and acquisition efficiency. This project addresses how to separate genuine performance signals from seasonal distortion, and what that means for acquisition strategy.

<br>

## 💡 Business Context
The GA4 Obfuscated Dataset looks at sales data from the Google Merchandise Store from November 2020 to January 2021. This dataset contains all information typically in a GA4 dataset, however some information has been redacted e.g. promotional campaign names and customer information in-line with data privacy requirements. 

<br>

## ✅ Executive Summary
The four days spanning Black Friday and Cyber Monday (BFCM) was the standout period with AOV hitting $82.77 against a $69.99 pre-BFCM baseline. In this period there was also a 6.6% discount-driven uplift suggesting customers are upgrading their baskets rather than simply buying the cheapest available item, an important distinction for how future promotions should be structured. The Post-Christmas period experiences a slump with revenue falling over 50% to $2,113 per day and AOV dropping to $64.02, making broad discounting and continued CPC spend during this window a margin cost without the volume to justify it. The user behaviour story is consistent across periods. New users made up 95% of traffic but converted at 23.4% versus 34.3% for returning users, with the gap most pronounced at view item and add-to-cart stages. A technical audit didn't surface any site issues, which points to onboarding and product-market fit rather than infrastructure — A/B testing on the first-visit experience is the logical next step to optimise conversion at these stages. When considering the effects of channels, CPC drove high engagement but experienced low AOV's with poor add-to-cart rates - functioning more like a discovery channel than a conversion channel. Referral is smaller in volume but consistently outperforms on intent and AOV, it is worth reviewing budget allocation to see if Referral would have a higher pay-off. The most underleveraged opportunity in the data is Canada, where BFCM AOV reached $95.28 versus $77.78 in the US. With just 8.2% of the overall BFCM traffic vs the US's 51% this suggests the opportunity is currently underdeveloped and worth exploring further.

<br>

## ⚙️ Tools & Analytical Skills Used
* **SQL (BigQuery)**: Unnesting, CTEs, window function, approx quantiles, funnel modelling, date formatting, safe divide
* **Tableau**:Table calculations, LODs, calculated fields, filters, dual axis 
* **Analytical Skills**:  Funnel analysis, seasonal decomposition, cohort analysis, segmentation analysis, channel attribution, statistical profiling


<br>

## 📊 Results & Recommendations
<br>

**1. BFCM is the best sales period seeing high volumes and high AOVs. Post-Christmas sees collapse in sales and AOV**
* AOV peaked during BFCM at $82.77 (vs a $69.99 baseline) with discounts driving a +6.6% uplift in order value. Suggests users upgrading during sales rather than searching for exclusively discounted items.
* Categories seeing biggest spikes in interest : Bags, Clearance, Branded Items, New Items, Small Goods and Writing Instruments (44%-107% increase on pre-BFCM). 
* Post-Christmas sees collapse in sales (down to $2,113 per day, >50% decrease from pre-BFCM period) and AOV (down to $64.02, an almost 10% decrease from pre-BFCM period). Suggest pivot to promoting high margin, low discount items Post-Christmas to prevent margins from collapsing.

<br>
<img width="1085" height="568" alt="Image" src="https://github.com/user-attachments/assets/c560ffcf-fe4c-4177-ac7f-b407a0d275bf" />

**Graph:** Shows peak AOV and sales per day during BFCM and slump during Post-Christmas period.

<br>

**2. New users made up the vast majority of users during this period, but they had significantly lower engagement and conversion rates compared to existing users.**
* New users exhibiting lower intent and lower engagement, with biggest drop offs in view item (22.5% New vs 43.7% Existing) and add to cart rates (18.9% New vs 30.7% Existing).
* View item worst in Christmas-Period (22%) and Post-Christmas-Period (17.8%).
* Add to cart worst in Pre-Christmas (7.4%) and Post-Christmas (16.9%).
* Technical audit ruled out site performance as a driver — drop-off patterns point instead to product-market fit and first-visit experience gaps, suggesting UX and onboarding interventions over infrastructure fixes - A/B test for best solutions.
<br>
<img width="1173" height="446" alt="Image" src="https://github.com/user-attachments/assets/74ab3371-86ee-464c-97ad-d51edf49f07a" />

**Graph:** Shows difference in conversion rates at each funnel stage showing new customers showing lower engagement at each stage of the funnel. Biggest drop offs for new customer at view item and add to cart.

<br>

**3. Organic the best performing channel overall. CPC spend should be focused on increasing awareness pre-BFCM, remarketing in BFCM. Expand referral programme**
* Organic is the best performer, driving 38-39% of traffic consistently. It is the most stable channel with the highest AOV across all periods, except for Christmas when referral had the highest AOV.
* Referral is lower volume (14% of traffic), but is a high intent channel. Specifically the link through "googlemerchandisestore.com" showed significantly higher AOV during the Post-Christmas period ($74.50). 
* CPC is high intent, low volume. CPC users had high add to cart rates pre-Black Friday but the lowest add to cart and AOV across the board. Suggests people are window shopping and converting later through Direct or Organic. Shift budget to remarketing in BFCM Period to customers who added to cart during pre-BFCM but didn't convert to purchase. Reduce CPC on broad keywords during post-Christmas period, not bringing in high-value customers.
<br>

<img width="2542" height="1232" alt="Image" src="https://github.com/user-attachments/assets/d8d8655b-ed3f-4651-bd2c-3526ebfd23fd" />
Graph: Shows organic is a consistently strong channel, with high traffic volume and high AOV. Shows referral peaks AOV during Post-Christmas period. CPC consistently low AOV, particulary in post-christmas slump.

<br>
<br>

**4. Canada has high AOVs during the BFCM, but is only 8% of traffic**
* Canada represents a high-value underinvested market with an AOV of $95.28 vs $77.78 in the US, yet is only 8.2% of the BFCM traffic compared to the US's 51% — suggesting significant upside from targeted localised spend during the November peak.

<br>

## 🚀 Next Steps

**1. Optimise the First-Visit Experience-** Launch A/B tests for first-purchase triggers (e.g. prompt to add to cart, personalised welcome offers) that aim to move new users from the homepage to the view item stage and from view item to add to cart stage.

**2. Expand Referral during the Post-Christmas Period and shift CPC budget to Remarketing in BFCM -** Increase budget to referral programme from CPC during the Post-Christmas period though the link "googlemerchandisestore.com". Shift CPC budget during BFCM to remarketing customers first landing on site and showing high levels of engagement during pre-BFCM.

**3. Scale the Canadian Market -** Explore localised promotional spend in Canada and develop targeted ads for the Canadian market during BFCM to capitalise on high AOV.
