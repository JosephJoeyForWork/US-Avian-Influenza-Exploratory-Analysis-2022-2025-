# Exploratory-Analysis-of-Avian-Influenza-Outbreak-Conditions-in-the-United-States-(2022-2025)-
### **Project Overview/Background**

With national attention surrounding Avian Influenza virus amid rising egg and poultry prices, understanding the spread of disease has become a matter of public interest. In response, an analysis was conducted using freely available government data, with the goal of finding actionable insights. These findings are intended to help inform farmers about the regions and conditions that require the most attention to mitigate the spread of disease among poultry flocks.

### **Project Objectives**

- Highlight which regions experience the greatest frequency of outbreaks and the most extensive spread of disease
- Analyze the frequency of outbreaks according to month and determine yearly trends
- Examine the affects of production type on outbreaks and transmission of disease

### **Data Description**

- **FlockByOutbreakDate**- Reference table listing confirmed poultry outbreak events between 2/12/2022-3/10/2025. Each entry includes the location of outbreak, the date it occurred, the number of outbreaks at that location, and the flock size (number of birds impacted).
- **BirdsAffectedByMonth**- Table including how many birds affected nationwide according to date (ranging from 12/1/24 to 3/23/25).
- **ConfirmedDate**- References dates of confirmed infections (2/12/2022-3/11/2025) by county, state and which production type the infected populations belonged to.
- **MapComparison**-Table detailing the contaminated bird populations across states, classified into backyard, commercial, and total flocks with corresponding outbreak totals and the most recent detection date (10/11/2022-3/11/2025).

### **Database Diagram**

https://dbdiagram.io/d/689baf2b1d75ee360a4dab76

### **Executive Summary**

**Since 2022**, outbreaks have shown an overall **downwards trend** with a clear high outbreak season between the months of **October** and **May** and a significant down season between the months of **June** and **September**. **December** alone accounted for **16%** of all outbreaks, with **November** contributing another **14%**. 

Government data reveals that **40%** of all outbreaks occurred in **WHOA Non-Poultry** farms, while **Commercial Turkey Meat Bird** accounted for an additional **26%**, and **WHOA Poultry** farms **11%**.

At the state level, **Minnesota**, **California**, **South Dakota**, and **Ohio** reported the highest number of outbreaks, collectively representing **35%** of all outbreaks nationwide. At the county level, **Sioux** (IA), **Weld** (CO), **Darke** (OH), and **Merced** (CA) experienced the most severe infection rates, together making up **8%** of total outbreaks. Notably, Sioux (IA) reported as few as five confirmed infections impacting over 12m birds.

### **Insights Deep Dive**

**Regional Insights**

Outbreaks were heavily concentrated in **Minnesota** (11% of total outbreaks), **California** (9%), **South Dakota** (9%), and **Ohio** (6%).  

The counties with the highest total outbreaks were **Mercer** (OH) with 47 outbreaks, **Lancaster** (PA) with 37, **Darke** (OH) with 24 , and **Merced** (CA) also with 24 .

![image.png](attachment:1a94b04d-ffb4-4060-ad44-962ac93a6f79:image.png)

The counties experiencing the most severe spread per outbreak were: **Sioux** (IA) with **5** outbreaks contaminating over **12m** birds, **Weld** (CO) with **17** outbreaks contaminating over **9.5m** birds, **Darke** (OH) with **23** outbreaks contaminating over **9m** birds, and **Merced** (CA) with **24** outbreaks contaminating over **8.7m** birds.

![image.png](attachment:eca9bb09-4965-4918-8b7e-37a64a6ac746:image.png)

**Production Insights**

**WOAH Non Poultry** totaled at **654** outbreaks accounting for **40%** of total outbreaks. The next most affected category is **Commercial Turkey Meat** with **423** outbreaks accounting for another **26%** of all outbreaks across farm varieties. 

It’s important to note that a single outbreak can be attributed to multiple production varieties. Consequently, outbreaks and infected flock sizes in the visualizations may be attributed to more than one production category. This overlap makes it impossible to completely isolate data for production types with fewer outbreaks from those with higher outbreak volumes.

![image.png](attachment:8769386d-9e85-4da1-a40f-35e849916b23:image.png)

**Seasonality**

The overall **trend** of outbreaks by year is **downward**. **2022** recorded the highest total outbreaks at **718**, while **2025** has the lowest total at **264** outbreaks (to the month of March). Monthly trends show **December** at the **peak** with an average of **87** outbreaks, whereas **August** sits at the **lowest** point with an average of just **8** outbreaks.

It’s worth emphasizing that the seasonal **highs and lows are not consistent** in duration and timing from year to year. On average, seasonal activity begins to **rise in October**, **peaks in December**, and starts **declining in May**; hitting its **lowest point** between **June and August**.

![image.png](attachment:acb2edf6-d4e6-4e4f-a826-105c57a9aed4:image.png)

### **Dashboard**

https://public.tableau.com/views/AvianInfluenzaOutbreaksAcrossUSFeb2022-Mar2025/Dashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

### **Recommendations**

Attention should be focused on the counties of **Sioux** (IA), **Weld** (CO), **Darke** (OH), and **Merced** (CA). These regions exhibit an unusual pattern: **large flocks** being c**ontaminated** by relatively **few outbreak** **incidents**. To understand this anomaly, more research is needed into factors such as the effect of **wild bird migration**, **density of flocks** compared to other regions, and the **effectiveness** of local farm **oversight protocols**.

**Minnesota**, **California**, **South Dakota**, and **Ohio** should dedicate resources to study farms’ operations and practices, especially considering these regions have experienced **notably higher outbreak rates** than others. Understanding the conditions in these farms, and why they are disproportionately affected, will be critical in **creating** more effective **prevention** and **intervention** strategies.

By managing wild bird migration and **forewarning** farmers of **peak migratory seasons**, poultry producers can better prepare for ‘bird flu season’ that data shows occurring between fall and spring. 

Further research into effective **wildlife deterrent methods** and **sanitation** based **prevention strategies** can significantly expand producers’ options for safeguarding their flocks during high risk periods.

### **Clarifying Questions/Caveats/Assumptions**

Because each instance of infection is often linked to multiple production types on the same farm, it’s not possible to perfectly separate the data of flock sizes by production. As a result, questions like which production types contaminate the most birds per outbreak remain largely unanswerable. Understanding this in more detail would give valuable insight into how different productions configurations affect the spread of disease.

The terms **“Birds Affected”** and **“Flock Size”** require further clarification; particularly regarding how the probability of contamination is determined. Understanding how that probability is assessed would give more insight into why some farms are so disproportionately affected by relatively few outbreaks.

### **Links to data sites used**

[Outbreak Locations](https://www.aphis.usda.gov/livestock-poultry-disease/avian/avian-influenza/hpai-detections/commercial-backyard-flocks)
