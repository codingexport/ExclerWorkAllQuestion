# ExclerWorkAllQuestion

# Tableau

## What is Tableau?

- **Tableau** is a leading data visualization tool used for data analysis and business intelligence.
- It helps in creating charts and dashboards to derive insights from source data.

## Example Dashboard

![Tableau Dashboard Example]( https://blog.coupler.io/wp-content/uploads/2024/07/ppc-multi-channel-dashboard-for-tableau-1024x587.png)
<!-- Replace the above URL with your own image link if needed -->
## Tableau products

 - **Tableau Desktop**: Dhasboards & Stories
 - **Tableau Server**: Publish and share
 - **Tableau online**: Publish & share in cloud platform
 - **Tableau Prep**: ETL activities
 - **Tableau Reader**: Just view others work
   
![]( https://intellipaat.com/mediaFiles/2015/11/tableau1.png )

# 📊 Tableau File Extensions - Explained

This document provides a list of commonly used Tableau file extensions along with a brief explanation for each. It is useful for anyone working with Tableau Desktop or Tableau Server and looking to understand the structure and purpose of each file type.

---

## 📁 Tableau File Extensions

| Extension | File Type                         | Description |
|-----------|----------------------------------|-------------|
| `.twb`    | Tableau Workbook                 | Contains visualization structure, formatting, and settings, but **not the data** itself. It is XML-based and requires access to the data source to display the visualizations. |
| `.twbx`   | Tableau Packaged Workbook        | A packaged version of `.twb` that includes the workbook and **all local data sources, images, and custom fonts**. Ideal for sharing visualizations. |
| `.tds`    | Tableau Data Source              | Contains metadata about a data source such as calculated fields, custom groups, bins, default properties, and joins. It does **not contain actual data**. |
| `.tdsx`   | Tableau Packaged Data Source     | A packaged version of `.tds` that includes the data source file and **local data**. Useful for sharing complete data connections. |
| `.tde`    | Tableau Data Extract (legacy)    | Extracted snapshot of the data optimized for fast performance. Replaced by `.hyper` in newer versions. |
| `.hyper`  | Tableau Hyper Data Extract       | The new and improved extract format introduced in Tableau 10.5. It's more efficient and supports larger datasets and faster query performance. |
| `.tms`    | Tableau Map Source               | Stores map service connection details, such as background maps or WMS connections. |
| `.tbm`    | Tableau Bookmark                 | Used to save individual worksheets (charts, dashboards, etc.) for reuse across workbooks. |
| `.tfl`    | Tableau Flow File                | Contains a Tableau Prep flow file (introduced in Tableau Prep), showing how data is cleaned, transformed, and prepared. |
| `.tflx`   | Tableau Packaged Flow File       | A packaged version of `.tfl`, which includes data files and resources needed for the Prep flow. |
![image](https://github.com/user-attachments/assets/1d2b9ef6-52b3-492a-bff9-c40a5046c3e7)

---

## 💡 Notes

- **Packaged files** (like `.twbx`, `.tdsx`, `.tflx`) are great for sharing with others who may not have access to the original data sources.
- **Extract files** (`.tde`, `.hyper`) are used to improve performance and support offline analysis.
- XML-based files like `.twb` and `.tds` can be opened with a text editor for debugging or version control purposes.

---
# 📊 Tableau - Data Source Overview

This README provides a summary of the **Data Source** section in Tableau, based on the attached diagram.

## 🔍 Overview
- The **Data Source** section is the **first screen** that appears after connecting Tableau to a data source.
- Users must **drag and drop tables** into the logical layer to begin analyzing the data.

---

## 🛠️ Operations Available:
1. **Rename**
2. **Copy Values**
3. **Hide/Unhide**
4. **Aliases**
5. **Create Calculated Field**
6. **Create Groups**
7. **Create Bins**
8. **Split**
9. **Custom Split**
10. **Pivot**
11. **Describe**

---

## 📁 Key Components:
- **Metadata**: Shows field types, physical table names, and more.
- **Data Preview Pane**: Displays a sample of data rows from the source table.

---

## 📌 Notes:
- You can switch between **Live** and **Extract** connections.
- You can add filters using the **Filters panel**.

---

## 📷 Image Reference:
Included image shows a sample data source setup using the "Orders (Sample - Superstore)" dataset.

![image](https://github.com/user-attachments/assets/2b8d203c-ef7e-4db4-a56a-aafdb163609f)

## Filter
![image](https://github.com/user-attachments/assets/fe3b6e8f-a9b1-4316-bde4-a75136e5b614)
![image](https://github.com/user-attachments/assets/ab6bd56f-dffe-46b7-9e51-d72b4fd03224)
# Tableau Filters, Data Modeling & Calculations – Interview Friendly Summary

This document provides a concise explanation of various important Tableau features, commonly asked in interviews for Data Analyst or BI roles. It includes types of filters, modeling features, and calculation functions.

---

## 🔍 Filters in Tableau

### 1. **Dimension Filter**
- Filters categorical data like Region, Category, etc.
- Applied before aggregation.
- ✅ *Example*: Filter only “East” and “West” regions.

---

### 2. **Measure Filter**
- Filters aggregated measures like SUM(Sales), AVG(Profit), etc.
- Applied after aggregation.
- ✅ *Example*: Filter sales greater than 10,000.

---

### 3. **Data Source Filter**
- Filters applied directly at the data source level.
- Helps with performance and security (e.g., row-level security).
- ✅ *Example*: Filter data for only the year 2023.

---

### 4. **Quick Filter (Show Filter)**
- A user-interface-based filter on the dashboard.
- Allows users to filter data using dropdowns or checkboxes.
- ✅ *Example*: Filter by product category on the dashboard.

---

### 5. **Context Filter**
- Applied first, sets the base for other filters.
- Improves performance and allows dependent filters.
- ✅ *Example*: Context filter on “East” region → apply Top N within East.

---

## 🧱 Data Modeling Features

### 6. **Hierarchy**
- Allows drill-downs in data (e.g., Year → Quarter → Month).
- ✅ *Example*: Sales per Year, drill down to Quarter.

---

### 7. **Group**
- Combine multiple dimension members into one group.
- ✅ *Example*: Combine “Phones” and “Laptops” into “Electronics”.

---

### 8. **Sets**
- Subset of data based on condition or manual selection.
- Types: Fixed Set & Dynamic Set.
- ✅ *Example*: Top 10 customers by Sales (dynamic set).

---

### 9. **Parameter**
- A dynamic input value controlled by the user.
- Can be used in filters, calculations, reference lines, etc.
- ✅ *Example*: Parameter to display Top N customers.

---

## 🧮 Calculations in Tableau

### 🥇 Top 3 Most Important Calculations

#### 1. **Calculated Field**
- Custom field created with a formula.
- ✅ *Example*: `IF [Profit] > 0 THEN "Profit" ELSE "Loss"`

#### 2. **Level of Detail (LOD) Expressions**
- Used to fix or change the level of aggregation.
- ✅ *Example*: `{FIXED [Customer Name] : SUM(Sales)}`

#### 3. **Table Calculations**
- Calculations based on table structure (e.g., % of total, running sum).
- ✅ *Example*: `RUNNING_SUM(SUM(Sales))`, `RANK(SUM(Profit))`

---

### 📌 Other Useful Calculations

| #  | Calculation Type         | Example / Use Case                           |
|----|--------------------------|----------------------------------------------|
| 4  | `IF / ELSEIF / ELSE`     | Conditional logic                            |
| 5  | `CASE` Statement          | Clean multi-condition replacement for IF     |
| 6  | `DATEDIFF` / `DATEADD`   | Date calculations                            |
| 7  | `LEFT()` / `RIGHT()`     | String manipulation                          |
| 8  | `ISNULL()` / `IFNULL()`  | Null handling                                |
| 9  | `ZN()`                   | Convert NULLs to 0                           |
| 10 | `RANK()` / `INDEX()`     | Rank / position in table                     |
| 11 | `WINDOW_SUM()`           | Aggregation across window                    |
| 12 | `% of Total`             | Proportional comparison                      |
| 13 | `IIF()`                  | Inline IF logic                              |
| 14 | `Z-Score`                | Outlier detection                            |
| 15 | `MIN()` / `MAX()`        | Aggregations                                 |
| 16 | `AVG()`                  | Average values                               |
| 17 | `SUM()`                  | Sum values                                   |
| 18 | `INT()` / `ROUND()`      | Numerical formatting                         |
| 19 | `FIND()`                 | Search substring in text                     |
| 20 | `NOW()` / `TODAY()`      | Current date/time                            |

---

## 📚 Summary

| Feature         | Key Role in Tableau                                      |
|----------------|----------------------------------------------------------|
| Dimension Filter | Filter data before aggregation                        |
| Measure Filter   | Filter data after aggregation                         |
| Data Source Filter | Secure and efficient filtering at source level      |
| Quick Filter     | UI component for dashboard interactivity              |
| Context Filter   | Foundation for dependent filters & performance        |
| Hierarchy        | Enables drill-downs                                    |
| Group            | Combine dimension values                               |
| Sets             | In/Out comparisons, subsets                            |
| Parameter        | Add interactivity with dynamic values                 |
| Calculations     | Build logic, KPIs, custom analytics                    |

---

> **Pro Tip for Interviews**: 
> Be ready to explain **when and why** you’d use one filter or calculation over another. Practice with use cases and sample dashboards!

---



## 📚 Additional Resources

- [Tableau File Types Documentation](https://help.tableau.com/)
- [Tableau Community Forums](https://community.tableau.com/)
