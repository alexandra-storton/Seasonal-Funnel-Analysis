# Seasonal-Funnel-Analysis-for-an-E-Commerce-Business

## 📌 Objective
To perform an end-to-end funnel analysis of a high-traffic retail dataset (GA4) during the Q4 sales peak, identifying how seasonal events — Black Friday, Cyber Monday, and Christmas —distort conversion behaviour and acquisition efficiency.

<br>

## 💡 Business Context
The GA4 Obfuscated Dataset looks at sales data from the Google Merchandise Store from November 2020 to January 2021. This dataset contains all information typically in a GA4 dataset, however some information has been redacted e.g. promotional campaign names and customer information for data-privacy issues. 

<br>

## ✅ Executive Summary
BFCM was the best performing period with an AOV of $82.77 and a +6.6% value uplift. This value collapsed Post-Christmas into a margin-eroding slump with revenue falling over 50% to $2,113 per day. To sustain growth, the focus must shift to bridging the new user engagement gap while scaling high-AOV opportunities in the Canadian market, shifting CPC strategy and referral channels.

<br>

**1. Capitalise on Black Friday & Cyber Monday (BFCM) sales spike.**
* AOV peaked during BFCM at $82.77 (vs $69.99 pre-BFCM), with discounts driving a +6.6% uplift in order value, suggests users upgrading during sales and not just looking to buy most discounted items.
* Post-Christmas slump where revenue drops by over 50% to $2,113 per day and AOV slides to $64.02 - reduce advertising and discounting, pivot to high-margin, low discount items to protect margin.

 <br>

**2.Bridge new user engagement gap.**
* Most users in this period (95%) were new users, however they converted at a significantly lower rate (23.4%) than returning users (34.3%).
* Biggest drop off from the view item stage (22.5% for new users vs 43.7% for existing) and the add to cart stage (18.9% vs 30.7%).
* No techincal issues found, instead product-market fit and seasonality issues - improve engagement and conversion features on site.

<br>

**3. Optimise Channel Mix & Expand into Profitable Areas.** 
* Referrals is a high-intent channel and brought in the highest AOV customers during the Post-Christmas Period ($74.50) - push this as an acquisition channel during this period through link googlemerchandisestore.com.
* CPC acts as a window shopping channel pre-BFCM with high engagement rates but poor add to cart rates (7%) and low final AOV. Remarket to these individuals during BFCM to capture those who added to cart or showed high engagement with site but didn't check out.
* Canada is an underinvested in market during BFCM, with the higest AOV of $95.28 vs the US's $77.78. Only 8.2% of traffic compared to the US's 51%.
  
<br>

## ⚙️ Tools Used
SQL (BigQuery): Unnesting, CTEs, Window Function, Statistical Profiling, Approx Quantiles, Funnel Modelling, Date Formating, Safe Divide

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
* New exhibiting lower intent and lower engagement, with biggest drop offs in view item (22.5% New vs 43.7% Existing) and add to cart rates (18.9% New vs 30.7% Existing).
* View item worst in Christmas-Period (22%) and Post-Christmas-Period (17.8%).
* Add to cart worst in Pre-Christmas (7.4%) and Post-Christmas (16.9%).
* No technical issues found - suggest improving user experience during first visit to site e.g. adding more first purchase triggers to encourage new users to buy/engage with site - A/B test for best solutions.
<br>
<img width="1173" height="446" alt="Image" src="https://github.com/user-attachments/assets/74ab3371-86ee-464c-97ad-d51edf49f07a" />

**Graph:** Shows difference in conversion rates at each funnel stage showing new customers showing lower engagement at each stage of the funnel. Biggest drop offs for new customer at view item and add to cart.

<br>

**3. Organic the best performing channel overall. CPC spend should be focused on increasing awareness pre-BFCM, remarketining in BFCM. Expand referral programme**
* Organic is the best performer, driving 38-39% of traffic consistently. It is the most stable channel with the highest AOV across all periods, except for Christmas when referral had the highest AOV.
* Referral is lower volume (14% of traffic), but is a high intent channel. Specifically the link through "googlemerchandisestore.com" showed significantly higher AOV during the Post-Christmas period ($74.50). 
* CPC is high intent, low volume. CPC users had high add to cart rates pre-Black Friday but the lowest add to cart and AOV across the board. Suggests people are window shopping and converting later through Direct or Organic. Shift budget to remarketing in BFCM Period to customers who added to cart during pre-BFCM but didn't convert to purchase. Reduce CPC on broad keywords during post-Christmas period, not brining in high-value customers.
<br>

<img width="2542" height="1232" alt="Image" src="https://github.com/user-attachments/assets/d8d8655b-ed3f-4651-bd2c-3526ebfd23fd" />
**Graph:** Shows organic is a consistently strong channel, with high traffic volume and high AOV. Shows referral peaks AOV during Post-Christmas period. CPC consistently low AOV, particulary in post-christmas slump.

<br>

**4. Canada has high AOVs during the BFCM, but is only 8% of traffic**
* Consider Canada as an area of expansion for BFCM, high AOVs $95.28 cs $77.78 in the US. Make up only 8.2% of BFCM market vs the US's 51% - explore localised promotional spend for the Canadian market during the November peak to capitalise on higher per-user spend.

<br>

## 🚀 Next Steps

**1. Optimise the First-Visit Experience-** Launch A/B tests for first-purchase triggers (e.g. prompt to add to cart, personalised welcome offers) that aim to move new users from the homepage to the view item stage and from view item to add to cart stage.

**2. Expand Referral during the Post-Christmas Period and shift CPC budget to Remarketing in BFCM -** Increase budget to referral programme from CPC during the Post-Christmas period though the link "googlemerchandisestore.com". Shift CPC budget during BFCM to remarketing customers first landing on site and showing high levels of engagement during pre-BFCM.

**3. Scale the Canadian Market -** Explore localised promotional spend in Canada and develop targeted ads for the Canadian market during BFCM to capitalise on high AOV.
