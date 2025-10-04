**Walmart Sales Data: Comprehensive Analysis and Strategic Decision-Making Report**



**Executive Summary**
This analysis of Walmart's weekly sales data from 2010-2012 reveals critical insights into seasonal trends, store performance, and the impact of external economic factors. Key findings include significant sales spikes during holiday periods, a strong negative correlation between unemployment and sales, and the ability to segment stores into three distinct performance clusters. The data provides a robust foundation for strategic decisions in inventory management, marketing, store operations, and financial forecasting. Implementing the recommended actions will optimize operations and drive revenue growth.



1. Data Overview and Preparation
The dataset is clean and well-structured, providing a solid foundation for analysis.

**Code:**

<img width="129" height="114" alt="image" src="https://github.com/user-attachments/assets/176d21b2-1f84-422d-a877-178035173e5e" />
 




<img width="232" height="110" alt="image" src="https://github.com/user-attachments/assets/45ea3176-7f77-4353-ba2d-bf9a86b4718f" />




 
**Output:**

<img width="350" height="91" alt="image" src="https://github.com/user-attachments/assets/0b356486-b50b-4b94-ae61-754a13dbd014" />




 
The data contains 6,435 records across 8 variables with no missing values or duplicates, ensuring the integrity of our analysis.

**Code:**

<img width="236" height="196" alt="image" src="https://github.com/user-attachments/assets/64fc3887-f0d8-469d-a33e-e7f8b74eedbb" />




 
**Output:**
 
<img width="424" height="303" alt="image" src="https://github.com/user-attachments/assets/76d46b7a-3fdb-4bd5-a562-4c65d88abe23" />





2. Strategic Planning & Financial Forecasting

Question: Based on the clear seasonal trends and quarterly patterns, how should we set our annual sales targets and allocate our budget for inventory and marketing across different quarters?

Analysis: We analyzed sales trends by month and quarter to identify seasonal patterns.

**Code:**

<img width="424" height="270" alt="image" src="https://github.com/user-attachments/assets/ca3d8568-42f8-4088-b7b4-b464cc933579" />
 
**Output:**

<img width="351" height="218" alt="image" src="https://github.com/user-attachments/assets/2b03d441-7ea6-4deb-9324-fc11acd0712a" />




 
**Yearly Sales:**

<img width="141" height="61" alt="image" src="https://github.com/user-attachments/assets/6b65f231-f508-4f38-8290-71d4dae53c59" />




 
**Quarterly Average Sales:**

<img width="390" height="61" alt="image" src="https://github.com/user-attachments/assets/01417756-8c9c-47ca-ae10-f28f841fa81d" />




 
**Findings & Recommendations:**

•	Q4 is Dominant: Sales in Q4 are consistently ~ 60% higher than in other quarters due to the holiday season (Thanksgiving, Christmas).
•	Steady Growth: Average sales show a slight year-over-year increase from 2010 to 2012 in Q1-Q3.
•	2012 Q4 Anomaly: 2012 Q4 sales were significantly lower than previous years; this warrants investigation into potential data or external factors.
**Informed Decisions:**
1.	Budget Allocation: Allocate 40-50% of the annual marketing and inventory budget to Q4 to capitalize on high demand.
2.	Inventory Planning: Work with suppliers to ensure stock levels are built up in late Q3 to meet Q4 demand.
3.	Target Setting: Set aggressive but achievable sales targets for Q4, while aiming for steady, incremental growth in Q1-Q3 based on the previous year's performance.

3. Store Operations & Performance Management

Question: Which stores are the top and bottom performers, and why is there such a significant variation?

Analysis: We ranked stores by total sales and analyzed their distributions.

**Code:**

<img width="308" height="221" alt="image" src="https://github.com/user-attachments/assets/658ab081-1b15-4c77-a84b-158e18911724" />




 
**Output:**

<img width="366" height="130" alt="image" src="https://github.com/user-attachments/assets/9e4ee44f-f39b-4d7c-844c-5a99a9bec118" />
 




**Diagram:**

<img width="366" height="220" alt="image" src="https://github.com/user-attachments/assets/d7e3bee9-1b48-45e4-9424-5355651fd1d2" />
 



<img width="366" height="220" alt="image" src="https://github.com/user-attachments/assets/4e3ad467-c2d1-4f26-a5d6-336877a2ee1e" />




 
**Findings & Recommendations:**
•	Significant Disparity: Store 20 is the top performer, with sales nearly double that of the lowest-performing stores.
•	Consistency: Some stores have high variance (whiskers on the boxplot are long), indicating inconsistent performance, while others are stable.
**Informed Decisions:**
1.	Benchmarking: Launch a project to identify best practices from Store #20, #4, and #14 (e.g., layout, local marketing tactics, staffing models) and implement them in lower-performing stores.
2.	Root Cause Analysis: Mandate a deep-dive analysis into the bottom 5 performing stores to determine causes: is it location, local competition, poor management, or store size?
3.	Performance Incentives: Tie store manager bonuses to both total sales and consistency (reducing variance), encouraging stable performance.

4. Marketing & Promotions

Question: Holidays have a statistically significant impact on sales. Which specific holidays drive the largest sales lifts?

Analysis: We compared sales on holiday vs. non-holiday weeks and measured the impact by month.

**Code:**

 <img width="366" height="300" alt="image" src="https://github.com/user-attachments/assets/f5eb93da-19d9-4af8-95fe-68c03224fdef" />





**Output:**

<img width="336" height="67" alt="image" src="https://github.com/user-attachments/assets/06df9b7a-cf00-4952-88c4-5c9546a1d7c4" />
 

 


<img width="194" height="47" alt="image" src="https://github.com/user-attachments/assets/d2ae655f-abbf-4b4a-9975-d24fac4ceaae" />
 




<img width="156" height="130" alt="image" src="https://github.com/user-attachments/assets/2f43c0e4-7c1d-419f-8ffd-8289ae441204" />





**Findings & Recommendations:**
•	Major Impact: Holiday weeks see ~24% higher sales on average than non-holiday weeks. The p-value of 0.0000 confirms this is not random.
•	Top Holidays: December (Christmas) and November (Thanksgiving) have the most significant impact by far.
**Informed Decisions:**
1.	Campaign Focus: Concentrate the most prominent marketing campaigns (TV, digital ads, circulars) around November and December.
2.	Promotional Planning: Plan "doorbuster" deals and major promotions for the weeks leading up to Thanksgiving and Christmas to capture the full wave of demand.
3.	Budget justification: Use the 24% sales lift metric to justify increased marketing spend during all holiday periods, not just year-end.

5. Economic Strategy & Risk Management

Question: How do external factors like Unemployment and CPI affect our sales?

Analysis: We calculated the correlation of external factors with Weekly Sales.

**Code:**

<img width="372" height="163" alt="image" src="https://github.com/user-attachments/assets/421bbca2-826f-46ef-beed-568bb84a8b76" />
 




**Output:**

<img width="243" height="48" alt="image" src="https://github.com/user-attachments/assets/9455c993-4aec-44d4-9d0c-7ecb8b53223b" />
 




**Diagram:**
 
<img width="258" height="217" alt="image" src="https://github.com/user-attachments/assets/33ba2657-ab27-4ae0-a6a4-f41b96f2928d" />





<img width="358" height="217" alt="image" src="https://github.com/user-attachments/assets/eac51179-13a8-4f1b-985d-094455228f6d" />





<img width="358" height="217" alt="image" src="https://github.com/user-attachments/assets/922b128b-c3bb-42a3-b80c-5b42d9d419b0" />




 
**Findings & Recommendations:**
•	Unemployment: Has a moderate negative correlation (-0.20) with sales. As unemployment rises, sales tend to fall.
•	CPI (Consumer Price Index): Has a moderate positive correlation (0.19). This may indicate that as the general cost of living rises, more people shop at Walmart for its value proposition.
•	Weak Influences: Temperature and Fuel Price have almost no linear correlation with weekly sales.
**Informed Decisions:**
1.	Recession Planning: Develop a contingency plan for economic downturns. This should include a focus on promoting essential goods and value brands to retain cost-conscious customers.
2.	Market Positioning: Leverage the positive CPI correlation in marketing messaging: "Walmart helps you fight inflation."
3.	Ignore Noise: Do not base pricing or promotion strategies on fluctuations in fuel prices, as there is no measurable impact on sales.

6. Time Series Analysis of Weekly Sales

Question: How did the weekly sales fluctuate over the year?

Analysis: The analysis reveals fundamental characteristic of Walmart's sales data:

**Clear and Predictable Seasonal Patterns:**
•	The decomposition shows strong, recurring yearly seasonality (period=52 weeks). This is visually evident as large, consistent peaks that occur at the same point each year (corresponding to the year-end holiday season around November/December) and troughs (e.g., in January).
•	The trend component is relatively stable or slightly increasing over the 2010-2012 period. There is no evidence of a sharp decline or explosive growth, indicating a steady business operation.
•	The residuals (the noise left after removing trend and seasonality) appear random. This means the additive model effectively captured the major patterns, and there are no obvious, unexplained events distorting the data.

**Code:**

<img width="231" height="217" alt="image" src="https://github.com/user-attachments/assets/d8429b0c-296c-4610-92c6-6c90e4b10cf9" />
 




**Output:**

<img width="264" height="136" alt="image" src="https://github.com/user-attachments/assets/446cb94c-74a6-453e-888d-7bcc2ecb1050" />
 




**Diagram:**
 
<img width="346" height="203" alt="image" src="https://github.com/user-attachments/assets/b553fce1-105e-45e1-8cac-0fa2368607b2" />





7. Store Clustering for Targeted Strategies

Question: Based on the K-means clustering, what are the profiles of the three distinct store clusters?

Analysis: We grouped stores into clusters based on their sales and economic characteristics.

**Code:**

<img width="208" height="315" alt="image" src="https://github.com/user-attachments/assets/060fcaef-45cd-43c5-b992-f39eeb0050ab" />
 




**Output:**

<img width="230" height="173" alt="image" src="https://github.com/user-attachments/assets/8a080cc3-4f16-452a-9417-ee3edc19cf47" />

 

 

<img width="431" height="71" alt="image" src="https://github.com/user-attachments/assets/daf5f870-d7df-44b9-b4cd-53744da8ac29" />

**Diagram:**

<img width="283" height="171" alt="image" src="https://github.com/user-attachments/assets/5f13b4d2-8855-400c-80f3-50ef0cfbbbf5" />

 


 
<img width="429" height="48" alt="image" src="https://github.com/user-attachments/assets/85838ebf-1ed3-4890-bfc8-fd4fc4d197c3" />





**Findings & Recommendations:**

•	Cluster 2 (High Performers): 16 stores with the highest sales and lowest unemployment. Affluent, high-volume locations.
•	Cluster 0 (Average Performers): 18 stores with mid-level sales and economic indicators.
•	Cluster 1 (Low Performers): 11 stores with the lowest sales and highest unemployment. Struggling economic areas.
**Informed Decisions:**
1.	Cluster-Specific Strategies:
	Cluster 2: Test new, premium products here first. Focus on customer experience and loyalty.
	Cluster 0: Implement best practices from Cluster 2 to drive growth. Focus on competitive pricing.
	Cluster 1: Optimize for value. Focus on essential goods and promote deep discounts. Assess the long-term viability of stores in severely economically depressed areas.
2.	Resource Allocation: Direct top managerial talent and renovation budgets to Cluster 2 and high-potential Cluster 0 stores to maximize ROI.


**Summary:** 

<img width="405" height="137" alt="image" src="https://github.com/user-attachments/assets/919604ac-4c7a-4d27-afde-24ed9b5510a3" />

 



<img width="189" height="106" alt="image" src="https://github.com/user-attachments/assets/6d75f311-f7d0-4914-b4f8-6c2f9d3b86d8" />
 

