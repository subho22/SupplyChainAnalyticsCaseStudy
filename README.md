# SupplyChainAnalyticsCaseStudy
 
Demand Data Analysis Exercise



Data Readme

	1. Download the data from following location
	
	2. There are four files:
		- Instruction 
		- DemandData.csv
		- Inventory.csv
		- SKUMaster.csv
		
	3. DemandData.csv: There are five data points provided for each SKU: 
		Retail: The Retail $ value of the sale
		GM$: The Gross Margin $ value of the sale
		Unit: The total units sold
		Weight: The weight of the total units sold
		Cube: The volume (in cubic meter) of the total units sold
		
	4. Inventory.csv: End of month inventory for every SKU

	5. SKUMaster.csv: For every SKU, following three fields are given:
		CategoryCode: SKU category used by the client internally. Every category has a category manager
		SKUStatus: Current status of the SKU. Consider only active SKU for all the analysis unless specified otherwise
		SupplierNumber: Supplier of this SKU
	
Analysis Questions

Q1. Normalize the inventory, and demand dataset for these columns (i.e make it flat dataset. each data item listed below should a column header)
	Demand Data: SKU, Month, Retail, GM, Units, Weight, Cube
	Inventory Data: SKU, Month, Units
	Focus on making this step repeatable. If the client changes the data in this format, one should be able to convert to into above format without much re-work.
	
Q2. Rank CategoryCodes and SupplierCodes in decreasing order of any of the five measures (Retail, GM, Units, Weight and Cube)

Q3. Calculate total average inventory by Category code and SupplierNumber in terms of RetailPrice, GM, Weight, Cube

Q4. Calculate the weighted average of RetailPrice, GM, Weight, and Cube per Unit from Demand Data. Apply these values as new columns in SKUMaster data. Calculate same values by CategoryCode and SupplierNumber and report them out.

Q5. In each CategoryCode, find the SKUs which make-up top 80% of volume in terms of RetailPrice. E.g. If there are 10 CategoryCodes, in each of the category code, find the SKUs which make up top 80% in terms of retailprice.

Q6. Analyse if there is any seasonality in overall volumes over the year; and also seasonality among CategoryCodes.

Q7. Calculate COV of Demand for each product COV (in units)=(Std.Dev of Units)/(Avg of Units). Create three clusters (Low, Med, High) in increasing order of COV with top 50% of units in Low, Next 30% in medium and bottom 20% in high.

Q8. Generate a pareto by SKU (in terms of retailprice) and see how many SKUs account for top 80%, next 15%, and bottom 5% of the sales



	







