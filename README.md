# :coffee: [Coffee Sales Dashboard]() :coffee:

### Project Description:

Analyze coffee sales data using **Excel** and create dashboard.
In this project, my primary aim was to 
- Practise excel functionalities which helps to clean and analyze dataset.
- Merge few tables data
- Uncover hidden insights of dataset.
- Visualize the statistics and patterns.


----------------------------------
### Key Components of the Project:

- [x] Data Preparation: :pencil:  :scissors:

:arrow_forward:Filled main worksheet by getting data from other work sheets.
      
:arrow_forward:Filled **Customer Name** from Order sheet

**=XLOOKUP(C2,customers!$A$2:$A$1001,customers!$B$2:$B$1001,,0)**

:arrow_forward:Filled **Email** from Order sheet

**=IF(XLOOKUP(C2,customers!$A$2:$A$1001,customers!$C$2:$C$1001,,0)=0,"",XLOOKUP(C2,customers!$A$2:$A$1001,customers!$C$2:$C$1001,,0))**
      
:arrow_forward:Filled **Country** from Order sheet

**=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$G$1:$G$1001,,0)**

:arrow_forward:Filled **All Product details** at once from Product sheet

**=INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!I$1,products!$A$1:$G$1,0))**

:arrow_forward:Filled **Sales**: Unit Price X Quantity

**=L2*E2**

:arrow_forward:Added new column **Coffee Type Name** and filed data 

**=IF(I2="Rob", "Robusta",IF(I2="Exc", "Excelsa", IF(I2="Ara", "Arabica", IF(I2="Lib","Liberica",""))))**
 
:arrow_forward:Added new column **Roast Type Name** and filed data

**=IF(J2="M", "Medium",IF(J2="L", "Light", IF(J2="D","Dark","")))**

:arrow_forward:Formatted **Order Date** to custom format dd-mmm-yyyy  

**9/5/2019 > 5 Sep 2019**

:arrow_forward:Formatted **Size** to custom format 0.0 Kg 

**0.5 > 0.5 Kg**

:arrow_forward:Change data type of  **Unit Price | Sales**  

:arrow_forward:Remove duplicates 



- [x] Data Analysis and Visualization: :bar_chart:
    
- Create pivot table for **"Average Income pre Purchase by Gender"** and generate **"Clustered Column Chart"**

![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/c954524a-a0a8-41f9-8b1b-0d0d1185bb9d)
![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/0687f643-8af8-4e4c-89b9-5ae8d76e82a5)


- Create pivot table for **"Purchasing by Commute Distance"** and generate **"Line Chart"**
  
![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/b286a06f-e37f-405a-ae0f-5d327212a148)
![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/33faf453-f9f1-4072-b8fb-6f4e830cdae8)

- Create pivot table for **"Purchasing by Commute Distance"** and generate **"Line with Markers Chart"**

![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/8920eb61-d5e9-46ba-ad97-92c44a3e03ce)
![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/c2d2856b-a311-4eb2-977a-44be55a2a70c)

- Created Dashboard and add Slicer for **Marital Status**

![image](https://github.com/hashinil/excel_Bike_Sales_Dashboard/assets/33922245/338fe889-45c4-415b-871a-6f147f1160d3)

- Then few cosmetic changes.
- :golf:

----------------------------------
### Technologies and Tools Used: 

- Excel

