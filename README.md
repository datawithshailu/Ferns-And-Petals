 # 🌸 **Ferns and Petals Sales Dashboard** 🌸  
*A data-driven analysis for a gifting company*

Ferns N Petals Sales Dashboard provides a comprehensive overview of key business metrics related to revenue, orders, and customer spending. Designed in Excel, the dashboard offers interactive insights into sales performance across different categories, occasions, and time periods.

## 📌 **Project Overview**
Ferns and Petals is a gifting company specializing in delivering gifts for various occasions like **Birthdays, Anniversaries, Raksha Bandhan, Holi, and Valentine’s Day**. This project involves creating a **dynamic sales dashboard** in Excel to analyze key business metrics, helping the company optimize its sales strategy and improve customer satisfaction.

## 🚀 **Process of Creating the Dashboard**
### **1️⃣ Data Extraction & Cleaning**
- Extracted raw data from multiple sources.
- **Removed whitespace** and checked for **distinct unique values** using column distributions.
- Ensured data integrity by verifying data types and missing values.

### **2️⃣ Data Transformation & Feature Engineering**
- Created a **new column for Month** extracted from the `Order_Date` to analyze **monthly revenue trends**.
- Extracted **Hour from Order Time** to understand peak order times.
- Created a **"Difference in Order Delivery"** column by calculating:  
  ```
  Delivery Date - Order Date
  ```
  Converted this to **days** to find the **average order delivery time**.
- Extracted **Hour of Delivery Time** to analyze the preferred delivery time slot.

### **3️⃣ Data Merging & Relationships**
- Merged **Order Table** and **Product Table** using **Joins** on a **common key (Product ID)** to get **Price in the Order Table**.
- Performed **data modeling using a Star Schema:**
  - **Customer ID** (One-to-Many Relationship)
  - **Product ID** (Primary Key)
- Created a **Revenue Column** using the formula:  
  ```excel
  Revenue = Order[Price] * Order[Quantity]
  ```
- Formatted `Order Date` to extract **day names** using:  
  ```excel
  =FORMAT(Orders[Order_Date],"DDDD")
  ```

### **4️⃣ Pivot Tables & Business Insights**
Based on business requirements, created **pivot tables** for:
- **Total Revenue**
- **Sales Performance by Month**
- **Top 5 Products by Revenue**
- **Top 10 Cities by Orders**
- **Order Quantity vs Delivery Time**
- **Revenue by Occasions**
- **Product Popularity by Occasion**

### **5️⃣ Visualization & Dashboard Creation**
- Developed an **interactive dashboard** with slicers for **Order Date, Delivery Date, and Occasion Filters**.
- Implemented **data protection** by locking the sheet.

## 📊 **Key Business Insights**
- Identified **seasonal revenue trends** with peak sales in **February and October**.
- Determined the **most popular product categories and cities with the highest orders**.
- Found the **average delivery time** and analyzed its impact on order volume.

## 🛠️ **Tools Used**
- **Excel (Power Query, Data Modeling, Pivot Tables)**
- **Data Cleaning & Transformation**
- **Joins & Relationships**
- **Data Visualization & Dashboarding**






