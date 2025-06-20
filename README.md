# Retail-Inventory-Optimization-Using-Excel-Lean-Principles


## Project Overview
This project aims at providing a low cost inventory control solution to small and medium companies(retail). While working for an automotive retail shop in the Democratic Republic of Congo, I found out that the shop didn't have an inventory control system which had a lot of repercusssion on the shop overall operations. Taking in consideration the limited resources that was at my disposition, I decided to provide a low cost solution to help the shop deal with the lack of inventory control system. As the company data is confidential, I simulated data similar to the original to showcase my solution

## Problem Statement
While working for the company and analyzing the whole process I noticed that the shop's overall functioning was severely hampered by a lack of proper inventory management practices, leading to a cascade of negative consequences.

### Key Problems:

#### Absence of Inventory Tracking System:
- No system to keep track of items in inventory.
- No inventory classification system.
- No tracking system for perishable goods.
#### Inadequate Sales Data Management:
- Sales records were kept on paper, making it difficult to compile a reliable sales data bank for forecasting future demand.

### Consequences of these Problems on Shop Functioning:

- Stockouts and Lost Sales: Certain items run out of stock without the knowledge of salespeople or management due to the lack of an inventory tracking system, directly resulting in lost customers.
- Inaccurate Demand Forecasting: The inability to compile solid sales data prevents effective forecasting of future demand, especially seasonal demand. This led to either inventory shortages (resulting in lost sales) or inventory excess (leading to holding costs and potential obsolescence).
- Lack of Inventory Visibility: Management was unable to ascertain the exact level of inventory at any given time, hindering informed decision-making.
- Loss of Perishable Goods: The absence of a dedicated tracking system for perishable goods directly leads to their loss due to spoilage or expiration.

The issues discovered are very comon among small to medium companies in most underdevelopped countries so the low cost solution could really come in handy for a lot of these small to medium retail shops.

### Project Goal
With the issues mentionned above, the goal of this project was to build a low-cost, scalable system to optimize inventory and reduce losses

## Methodology
### Data Collection
#### Initial Data Collection
The initial data collection consisted of listing all items sold at the shop and creating a product list sheet in Excel and then performing a physical stockcount to determine the initial stock level of all items. As a result of this process, an Excel sheet ***Product_List*** was created with the following columns: `Product_ID`,	`Product_Name`,	`Unit`,	`Price`,	`Quantity`, and	`Notes`.


![image](https://github.com/user-attachments/assets/b1ce786c-4328-4a1b-915d-7f99672c5417)

      
#### Inventory inflow and outflow data collection
- To collect inventory inflow which refers to the acquisition of merchandise in the business, an ***Inflow*** sheet was created with the following columns:
`Date`,	`Product_ID`,	`Product_Name`,	`Unit`, and `Quantity`

![image](https://github.com/user-attachments/assets/7b00223e-ffb9-4118-9a23-2f5af1f199b3)

The Columns `Product_Name` and	`Unit` are autofilled using *VLOOKUP* with the ***Product_List*** sheet as the loolup array and column `Product_ID` as lookup value. What this does is that when there's an Inventory Inflow, the user will just enter the product ID in the the column `Product_ID` and columns `Product_Name` and `Unit` will be autofilled with information linked to the product ID typed. The user will then just enter the quantity in the quantity column.

**NOTE:** I used VLOOKUP back then as I didn't know *XLOOKUP* existed but *XLOOPUP* can be used here and is in fact simplier than *VLOOKUP*.

- To collect inventory outflow 2 sheets were created; the ***Outflow*** sheet to store outflow of inventory going to others shops and the ***Sales*** sheet to store sales data.
  

![image](https://github.com/user-attachments/assets/adbe46bd-a4ea-408c-adb0-23c48821f447)


Cell referencing was also used here to make data entry easy.
