# 🐔 Give a Cluck and Donate

**An exploration of food access gaps using socio-economic data and store locations to identify U.S. communities that may benefit most from Vital Farms product donations.**  
*Built with Python & Tableau*

---

## 📌 Quick Links
-  [**Interactive Tableau Dashboard**](https://public.tableau.com/views/VitalFarmsDonationDashboard/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 

---

## 🐣 Background

In their 2024 Impact Report, **Vital Farms** highlighted impressive efforts to support communities in need, donating:

- 💰 $110,000 in donations  
- 🍳 4.4 million eggs  
- 🧈 713,244 lbs of food donated
- 💵 $855,516 equivalent in food donated

As part of their mission to practice **Conscious Capitalism**, the company emphasizes giving back. This project aims to support that mission by helping visualize and prioritize areas across the U.S. where **Vital Farms' donations could make the greatest impact**.

This project identifies ZIP codes with high poverty rates and limited access to **premium retailers** (e.g., Whole Foods and Sprouts) as indicators of potential need. The resulting dashboard — titled *"Give a Cluck and Donate"* — offers data-driven insights into which regions might benefit most from future food donations.

---

## 📊 The Data

The project combines multiple data sources:

-  **Socioeconomic Data by ZIP Code**  
  (originally collected for a Trader Joe’s location analysis)  
  - Poverty rates  
  - Population counts  
  - Geographic info

-  **Store Locations**  
  - Whole Foods and Sprouts store addresses and ZIP codes  
  - These act as **proxies for high-income food retail access**

-  **Python Script**  
  A Jupyter Notebook was used to:
  - Clean and merge store and demographic data  
  - Classify ZIP codes into **Donation Need Categories**:  
    - High (≥50% poverty)  
    - Moderate (25–49%)  
    - Low (<25%)  
  - Output a clean dataset for Tableau visualization

---

## 📈 The Dashboard: *Give a Cluck and Donate*

> This interactive dashboard highlights areas with high poverty and low access to premium Vital Farms retailers — helping prioritize locations for future food donations.
![Dashboard Screenshot](/images/Dashboard.png)

###  **Map of High-Need ZIP Codes**
![Map Screenshot](/images/map.png)  
*A geographic visualization of ZIPs with >50% poverty. Darker and larger dots indicate more severe poverty.*

---

###  **Premium Retailers by State**
![Treemap Screenshot](/images/treemap.png)  
*Treemap showing number of Whole Foods and Sprouts by state — an indicator of where premium food access already exists.*

---

###  **Donation Need vs Retail Access**
![Bar Chart Screenshot](/images/barchart.png)  
*A comparison of donation need levels and the corresponding number of premium retailers available in those areas.*

---

## 🔗 Future Enhancements
- Integrate **Vital Farms retail partner list** beyond Whole Foods/Sprouts for more complete coverage
- Layer in **food desert data** from USDA
- Add ZIP-level population weights for deeper need prioritization
