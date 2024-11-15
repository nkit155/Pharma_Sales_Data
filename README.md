# Pharma Sales Analysis

## Decription:
This project is about to pharma company.it's business spread in two country's.in which company has many product as well as distributor where product supply to different channel, sales representative of company sales generate of this products.with the help of this project analysis how we can increase revenue of this company as focus on those products who not more generate revenue as per expectations and which sales team doing excellent perfomance and in whic channel company need increase supply.


## Data Source and Cleaning:
this dataset has one excel file.with the help of data cleaning function we can check data types of every column  **print(df.dtypes)**  and aslo check missing value **print(df.isnull().sum())** and how much column and row in database **print(df.shape)**  .therefore we check, if datatypes is wrong we can not properly calculate and analysis so got the wrong result. 

## Key Insights:
- Step 1: **Delta Team highest generate sales**
-  data['Sales Team'].value_counts().reset_index()
- Step 2:  **Ionclotide product of highest maximum price** 
- highest_sales_customer=data.loc[data['Sales'].idxmax()]
- Step 3: **Pharmacy has greater involvement in the business**
- channel_prod_count=data.groupby('Channel').agg(prod_count=('Product Name','count'))
-  channel_prod_count
-  Hospital	 124111
-  Pharmacy	 129971
- Step 4: **Average price of product**
-  data['Price'].mean()
-  412.2077203422517
- Step 5: **Germany is more involement than polland**
-   country_data=data['Country'].value_counts().reset_index()
-   Country	  count
-  	Germany	  213598
-   Poland	  40484

- ## Dashboard/Reports:
- Step 1: **Top 5 Product using bar chart:**
- ![Screenshot 2024-11-15 181515](https://github.com/user-attachments/assets/e24d8ce9-7d51-457b-a92c-7a78d861ffa2)
- Step 2: **Between corelation price and quantity using scatter plot with the help of matplotlib.
- ![Screenshot 2024-11-15 182027](https://github.com/user-attachments/assets/0921d938-e438-48d5-9058-15a5b39a8d95)
- Step 3: **Show box plot between price and product class**
- ![Screenshot 2024-11-15 182632](https://github.com/user-attachments/assets/3329a1d4-76a4-4309-a640-b0474ca159e5)
- Step 4: **Pharmacy genrate more sales than hospital by using box plot**
- ![Screenshot 2024-11-15 182921](https://github.com/user-attachments/assets/bf571eac-e864-411f-9a76-131841fd325c)
- Step 5: **Price distribution using histogram plot**
- ![Screenshot 2024-11-15 183107](https://github.com/user-attachments/assets/6c22a81b-fbe9-42b2-aa4a-88ad0065430c)





   
  


- 
