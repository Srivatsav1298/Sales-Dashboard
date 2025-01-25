# **Sales Dashboard**

---

## **Overview**

The Sales Dashboard project provides an interactive web-based interface to analyze supermarket sales data. Built with Streamlit, this dashboard allows users to filter and explore sales data based on various parameters such as city, customer type, and gender. The dashboard features key performance indicators (KPIs), visualizations of sales by product line, and hourly sales trends.

The main goal of this project is to provide decision-makers with an easy-to-use platform to assess sales performance and uncover trends, helping optimize sales strategies and improve business operations.

---

## **Features**

1. **Dynamic Filtering**:
   - Filter data by city, customer type, and gender using the sidebar.
   - Interactive selection with real-time updates.

2. **Key Performance Indicators (KPIs)**:
   - Displays total sales, average rating, and average sales per transaction.
   - Visual representation of ratings using star icons.

3. **Visualizations**:
   - Bar charts showcasing sales by product line and sales by hour.
   - Interactive charts powered by Plotly for detailed analysis.

4. **Sales Insights**:
   - Insights on product line performance and hourly sales trends.
   - Supports real-time updates based on the selected filters.

5. **Data Processing**:
   - Uses Pandas to read and process Excel data efficiently.
   - Caching implemented for faster data retrieval.

6. **Streamlit Integration**:
   - Built with Streamlit for an interactive and user-friendly interface.
   - Custom styling to hide Streamlit's default UI components.

---

## **Technical Details**

### **Input and Output**
- **Input**:
  - Excel file (`supermarket_sales.xlsx`) containing sales data.
  - Data is read from the `Sales` sheet, with selected columns processed for visualization.
- **Output**:
  - Interactive dashboard with various plots and KPIs.

### **Key Components**
- **Data Import**: 
  - Data is read using `pandas.read_excel` with customized column and row selections.
  - A new "hour" column is added based on the time of transaction.
- **Streamlit Widgets**:
  - Sidebar contains multiselect widgets for city, customer type, and gender.
  - Real-time filtering based on user selections.
- **Visualization**:
  - **Bar charts** generated using Plotly Express to visualize sales by product line and by hour.
  - Customization of chart styles for a cleaner user interface.

---
