# 🧭 Sales Compass - Interactive Power BI Dashboard

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=black)](https://powerbi.microsoft.com/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)



## 📊 **Live Dashboard Preview**


<img width="797" height="444" alt="image" src="https://github.com/user-attachments/assets/0ef99d23-555e-4d69-8928-b647bf4d46de" />




## 🎯 **Project Overview**

**Sales Compass** is an interactive Power BI dashboard designed to track and analyze online sales data. This comprehensive analytics tool provides real-time insights into sales performance, profitability, customer behavior, and regional trends, helping businesses make data-driven decisions.

### **What Makes This Dashboard Unique?**

| Feature | Benefit |
|---------|---------|
| 🧭 **Strategic Navigation** | Like a compass, it guides decision-making with clear direction |
| 📊 **Real-time Insights** | Interactive filters for instant analysis across dimensions |
| 💰 **Profit Optimization** | Identify profitable products, regions, and customer segments |
| 👥 **Customer Intelligence** | Understand buying patterns, preferences, and loyalty |
| 📈 **Growth Tracking** | Monitor trends, identify seasonality, and forecast performance |

---

## 🚀 **Key Features**

### 1. Interactive Dashboard
- Real-time KPIs: Sales, Profit, Orders, Quantity
- Average Order Value (AOV) & Profit Margin %
- Loss Making Orders identification
- Business Health Score (0-100)

### 2. Advanced Filtering & Slicers
- **Category** filter for product analysis
- **State** filter for regional insights
- **Payment Mode** filter for channel analysis
- **Date Range** slicer for time-based analysis
- **Customer** filter for individual performance

### 3. Customized Visualizations
- **Bar Charts** - Category performance comparison
- **Pie Charts** - Sales distribution by category
- **Donut Charts** - Payment mode breakdown
- **Clustered Bar Charts** - State vs Category matrix
- **Scatter Charts** - Profit vs Sales analysis
- **Line Charts** - Monthly/Yearly trends
- **Area Charts** - Cumulative sales tracking
- **Maps** - Geographic sales distribution
- **Slicers** - Interactive filtering controls

### 4. Drill-Down Capabilities
- Click on any visual to drill down to detailed views
- Hierarchical navigation from State → City → Customer
- Category → Sub-Category → Product analysis
- Explore data from summary to granular level

### 5. Data Manipulation & Calculations
- Advanced DAX calculations for complex metrics
- Custom measures for business-specific KPIs
- Calculated columns for enriched analysis
- User-driven parameters for flexible analysis

### 6. Data Integration
- Connected multiple data sources
- Joined tables for comprehensive analysis
- Created relationships for seamless data flow
- Implemented star schema for optimal performance

---

## 📁 **File Structure**

```
Sales-Compass-Dashboard/
│
├── 📊 Reports/
│   └── Sales Compass.pbix              # Main Power BI dashboard file
│
├── 📂 Data/
│   ├── Orders.csv                       # Order-level data
│   └── Details.csv                      # Product-level data
│
├── 🖼️ Images/
│   ├── Dashboard_Preview.png            # Main dashboard view
│   ├── Category_Analysis.png            # Category performance view
│   ├── Geographic_Insights.png          # Regional analysis view
│   ├── Payment_Analysis.png             # Payment mode analysis view
│   └── Customer_Insights.png            # Customer analytics view
│
├── 📝 Documentation/
│   ├── Data_Model_Overview.pdf          # Data model documentation
│   ├── User_Guide.pdf                   # How to use the dashboard
│   └── Business_Questions.pdf           # Key business questions answered
│
└── 📄 README.md                         # This file
```

---

## 🛠️ **Tech Stack**

| Tool | Purpose |
|------|---------|
| ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=Power%20BI&logoColor=black) | Dashboard development & visualization |
| ![DAX](https://img.shields.io/badge/DAX-Advanced-blue?style=flat-square) | Complex calculations & measures |
| ![Power Query](https://img.shields.io/badge/Power%20Query-M%20Language-6B8E23?style=flat-square) | Data transformation & ETL |
| ![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white) | Source data preparation |

---

## 🗂️ **Data Model**

```
┌─────────────────────────────────────────────────────────────┐
│                      Orders (1)                            │
├─────────────────────────────────────────────────────────────┤
│ ║ Order ID (Primary Key) ║                                │
│   Customer Name                                            │
│   Order Date                                               │
│   State                                                    │
│   City                                                     │
└────────────────────┬────────────────────────────────────────┘
                     │
                     │ 1 : * (One-to-Many)
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│                     Details (*)                            │
├─────────────────────────────────────────────────────────────┤
│ ║ Order ID (Foreign Key) ║                                │
│   Amount                                                   │
│   Profit                                                   │
│   Quantity                                                 │
│   Category                                                 │
│   Sub-Category                                             │
│   PaymentMode                                              │
└─────────────────────────────────────────────────────────────┘
```

### Relationship Details:
- **Cardinality:** Many to One (*:1)
- **Cross Filter Direction:** Single (Details filters Orders)
- **Active Relationship:** Yes

---

## 📊 **Project Learnings**

### 1. Interactive Dashboard Creation
- Designed and developed an interactive dashboard to track and analyze online sales data
- Implemented user-friendly navigation for seamless data exploration
- Created a cohesive visual story from raw data to actionable insights

### 2. Advanced Filtering & Parameters
- Used **complex parameters** to enable drill-down capabilities in worksheets
- Implemented **customization** using filters and slicers for user-driven analysis
- Created dynamic parameters that adapt to user selections
- Enabled multi-dimensional data exploration

### 3. Data Integration & Manipulation
- **Created connections** between multiple data sources
- **Joined new tables** to enrich the data model
- Implemented **calculations** to manipulate data and derive insights
- **User-driven parameters** for flexible visualization customization

### 4. Visualization Design
- Used **different types of customized visualizations:**
  - 📊 **Bar Chart** - Comparing category performance
  - 🥧 **Pie Chart** - Showing sales distribution
  - 🍩 **Donut Chart** - Payment mode breakdown
  - 📊 **Clustered Bar Chart** - State vs Category analysis
  - ⚫ **Scatter Chart** - Profit vs Sales correlation
  - 📈 **Line Chart** - Monthly/yearly trends
  - 🟦 **Area Chart** - Cumulative performance
  - 🗺️ **Map** - Geographic sales distribution
  - 🎯 **Slicers** - Interactive filtering controls

### 5. Business Intelligence Capabilities
- Real-time KPI monitoring
- Trend analysis and forecasting
- Segment-wise performance tracking
- Profitability analysis across dimensions
- Customer behavior insights

---

## 📸 **Dashboard Screenshots**

### 1. Executive Summary Dashboard
*(Add your screenshot here)*

*Key metrics at a glance with high-level performance overview*

---

### 2. Category Performance Analysis
*(Add your screenshot here)*

*Detailed analysis of sales, profit, and trends by product category*

---

### 3. Geographic Insights View
*(Add your screenshot here)*

*State and city-wise performance with geographic mapping*

---

### 4. Payment Channel Analytics
*(Add your screenshot here)*

*Payment mode distribution, profitability, and adoption trends*

---

### 5. Customer Intelligence
*(Add your screenshot here)*

*Customer segmentation, top customers, and loyalty analysis*

---

### 6. Time Intelligence View
*(Add your screenshot here)*

*Monthly, quarterly, and yearly trends with growth indicators*

---

## 🚀 **Quick Start Guide**

### Prerequisites
- Power BI Desktop (May 2023 or later)
- Basic understanding of Power BI (recommended)

### Installation Steps

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/Sales-Compass-Dashboard.git

# 2. Navigate to the project folder
cd Sales-Compass-Dashboard

# 3. Open the dashboard in Power BI
start Reports/"Sales Compass.pbix"
```

### How to Use

1. **Open the Dashboard**
   - Launch Power BI Desktop
   - Open the `Sales Compass.pbix` file

2. **Explore Interactively**
   - Click on any visual to cross-filter other visuals
   - Use the slicers to filter by Category, State, Payment Mode, or Date
   - Hover over charts for detailed tooltips

3. **Drill Down**
   - Double-click on any chart element to drill down
   - Right-click for drill-through options
   - Explore data from summary to granular level

4. **Refresh Data**
   - Go to `Home` → `Refresh` to update with latest data
   - Or click `Transform Data` to modify queries

5. **Customize**
   - Add your own measures using DAX
   - Modify visuals to suit your needs
   - Add new data sources as required

---

## 💡 **Sample Business Questions Answered**

| Business Question | How Dashboard Answers |
|-------------------|----------------------|
| **Which categories drive the most revenue?** | Category Contribution % with Sales by Category chart |
| **Which states are underperforming?** | State Sales Rank with Geographic map |
| **Who are our top customers?** | Top Customer measure with Customer Ranking |
| **Is digital payment adoption growing?** | Digital Payment % with trend over time |
| **Is our business healthy?** | Business Health Score with KPI indicators |
| **What are seasonal trends?** | Monthly Sales Trend with growth indicators |
| **Which products are most profitable?** | Category & Sub-Category Profit Margin analysis |
| **What payment modes are preferred?** | Payment Mode Distribution with donut chart |

---

## 🎯 **Key Achievements**

- ✅ **Interactive Dashboard** with real-time data tracking
- ✅ **Advanced Filtering** with complex parameters and slicers
- ✅ **Multiple Visualizations** with 10+ chart types
- ✅ **Data Integration** with connections and table joins
- ✅ **Calculations & Parameters** for user-driven analysis
- ✅ **Drill-Down Capabilities** for detailed exploration
- ✅ **Profit Optimization** through comprehensive analytics
- ✅ **Customer Intelligence** for loyalty and retention
- ✅ **Geographic Analysis** with state and city insights
- ✅ **Time Intelligence** for trend and seasonality analysis

---

## 📚 **Visualizations Used**

| Visualization | Purpose | Example Use Case |
|---------------|---------|------------------|
| 📊 **Bar Chart** | Comparison | Category performance comparison |
| 🥧 **Pie Chart** | Distribution | Sales distribution by category |
| 🍩 **Donut Chart** | Distribution with total | Payment mode breakdown |
| 📊 **Clustered Bar** | Multi-dimensional | State vs Category analysis |
| ⚫ **Scatter Chart** | Correlation | Profit vs Sales relationship |
| 📈 **Line Chart** | Trends | Monthly sales trends |
| 🟦 **Area Chart** | Cumulative | Cumulative sales over time |
| 🗺️ **Map** | Geographic | State-wise sales distribution |
| 🎯 **Slicers** | Filtering | Interactive category/state filters |
| 📊 **Card Visuals** | KPIs | Total Sales, Profit, Orders |

---

## 🔄 **Version History**

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | August 2026 | Initial release with complete dashboard |
| v1.1 | *Planned* | Advanced forecasting & predictive analytics |
| v1.2 | *Planned* | Real-time data integration |
| v2.0 | *Planned* | Mobile-responsive design |

---

## 🤝 **Contributing**

Contributions are welcome! Here's how you can help:

### Ways to Contribute
1. 🐛 **Report Bugs** - Open an issue
2. 💡 **Suggest Features** - Submit ideas
3. 📝 **Improve Documentation** - Update README
4. 🎨 **Enhance Visualizations** - Add new charts
5. 📊 **Add New Measures** - Share DAX code

### Contribution Process
```bash
# 1. Fork the repository
# 2. Create a feature branch
git checkout -b feature/AmazingFeature

# 3. Commit changes
git commit -m 'Add some AmazingFeature'

# 4. Push to branch
git push origin feature/AmazingFeature

# 5. Open a Pull Request
```

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 **Acknowledgments**

- Data source: Sample sales dataset
- Power BI Community for inspiration
- [Any other acknowledgments]

---

## 📞 **Connect With Me**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourusername)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your.email@example.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=About.me&logoColor=white)](https://yourportfolio.com)

---

## ⭐ **Support This Project**

If you find this project helpful:
- ⭐ **Star** the repository
- 🔄 **Fork** it for your needs
- 📢 **Share** with your network
- ✍️ **Submit** issues or suggestions

---

## 📊 **Dashboard Preview Animation**
For quarter 1
<img width="795" height="443" alt="image" src="https://github.com/user-attachments/assets/32f6f743-7992-4b30-b5ee-222c1c6337f7" />


---

## 🎯 **Ready to Navigate Your Sales Data?**

**Sales Compass** helps you find your way to better business decisions!

---

**Made with ❤️ using Power BI**

*Version 1.0 | August 2026*
