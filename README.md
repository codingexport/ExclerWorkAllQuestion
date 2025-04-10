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

---

## 💡 Notes

- **Packaged files** (like `.twbx`, `.tdsx`, `.tflx`) are great for sharing with others who may not have access to the original data sources.
- **Extract files** (`.tde`, `.hyper`) are used to improve performance and support offline analysis.
- XML-based files like `.twb` and `.tds` can be opened with a text editor for debugging or version control purposes.

---

## 📚 Additional Resources

- [Tableau File Types Documentation](https://help.tableau.com/)
- [Tableau Community Forums](https://community.tableau.com/)
