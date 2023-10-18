# :coffee: [Coffee Sales Dashboard](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/blob/main/CoffeeSalesDashboard.xlsx) :coffee:
![image](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/assets/33922245/741bec87-7153-48e8-974d-3e1594f89a3e)

### :pushpin: About Project:

Analyze coffee sales data using **Excel** and create dashboard.

In this project, my primary aim was to 

**:mag: Find:**

- Total sales over time
- Sales by Country
- Top 5 customers

**:dart: Practise**

- Excel functionalities which helps to clean and analyze dataset.
- Merge few tables data
- Uncover hidden insights of dataset.
- Visualize the statistics and patterns.


----------------------------------


### :pushpin: Key Components of the Project:


**:scissors: Data Preparation:** 


1. Filled main worksheet by getting data from other work sheets.
1. Filled **Customer Name** from Order sheet

      - [x] **=XLOOKUP(C2,customers!$A$2:$A$1001,customers!$B$2:$B$1001,,0)**

1. Filled **Email** from Order sheet

      - [x] **=IF(XLOOKUP(C2,customers!$A$2:$A$1001,customers!$C$2:$C$1001,,0)=0,"",XLOOKUP(C2,customers!$A$2:$A$1001,customers!$C$2:$C$1001,,0))**
      
1. Filled **Country** from Order sheet

      - [x] **=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$G$1:$G$1001,,0)**

1. Filled **All Product details** at once from Product sheet

      - [x] **=INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!I$1,products!$A$1:$G$1,0))**

1. Filled **Sales**: Unit Price X Quantity

      - [x] **=L2*E2**

1. Added new column **Coffee Type Name** and filed data 

      - [x] **=IF(I2="Rob", "Robusta",IF(I2="Exc", "Excelsa", IF(I2="Ara", "Arabica", IF(I2="Lib","Liberica",""))))**
 
1. Added new column **Roast Type Name** and filed data

      - [x] **=IF(J2="M", "Medium",IF(J2="L", "Light", IF(J2="D","Dark","")))**

1. Added new column **Loyality Card** and filed data

      - [x] **=XLOOKUP([@[Customer ID]],customers!$A$1:$A$1001,customers!$I$1:$I$1001,,0)**

1. Formatted **Order Date** to custom format dd-mmm-yyyy  

      - [x] **9/5/2019 > 5 Sep 2019**

1. Formatted **Size** to custom format 0.0 Kg 

      - [x] **0.5 > 0.5 Kg**

1. Change data type of  **Unit Price | Sales**

      - [x] **USD**

1. Remove duplicates 


**:bar_chart: Data Analysis and Visualization:** 

1. Create table

      - [x] Select all data and **Ctrl+t**

1. Name your table.
   
      ![image](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/assets/33922245/77ca97a5-98d0-4b52-901f-15d38d0b6a7a)
    
1. Create pivot table, re-name the sheet **TotalSales**, re-name the pivot table **TotalSales**. Add line chart, Timeline filter and do cosmetic Changes.

      ![image](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/assets/33922245/f95cc854-f6d4-4d83-969d-b225740c2854)

1. Take a Copy of pivot table and rename Sheet **CountryBarChart**

      ![image](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/assets/33922245/9d0e77dd-0b93-4800-acb4-b0628cc830be)

1. Take a Copy of pivot table and rename Sheet **Top5Customers**

      ![image](https://github.com/hashinil/excel_Coffee_Sales_Dashboard-Public/assets/33922245/8bd035c2-f86e-4786-96a6-78560b7aed35)

1. Created New worksheet and named it **Dashboard**
   
1. Then Copied all charts created, applied filters for all charts and did few cosmetic changes.

:golf:

----------------------------------
### :pushpin: Technologies and Tools Used: 

- Excel

