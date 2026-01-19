[India Healthcare Dashboard]
(Visualizations/Hospital_Dashboard1.png)

India Healthcare Infrastructure Analysis (2026)
📌 Project Overview
This project provides a comprehensive analysis of India's healthcare infrastructure, focusing on the distribution of hospital facilities and bed capacities across different States and Union Territories. The analysis highlights the disparity between Urban and Rural healthcare resources to assist in data-driven decision-making for infrastructure development.

Key Metrics Tracked:
Total Healthcare Facilities: 24K

Total Urban Beds: 431K

Total Rural Beds: 280K

Total Urban Hospitals: 3772

Total Rural Hospitals: 20K

📂 Project Structure
The project is organized into the following directory structure:

/Data: Contains the raw and cleaned datasets (CSV/Excel).

/Scripts: Jupyter Notebooks used for initial data cleaning and preprocessing.

/Visualizations: Power BI .pbix file and dashboard screenshots.

/Documentation: Detailed PDF report of the analysis.

🛠️ Tools & Technologies
Jupyter Notebook (Python): Used for initial data cleaning and handling missing values.

Power BI: Used for data modeling, DAX calculations, and interactive visualization.

Power Query: Used for final data transformation and date type formatting.

DAX (Data Analysis Expressions): Used to create custom measures like Total Facilities.

🧼 Data Cleaning Process
Before visualization, the data underwent several cleaning steps:

Handling Missing Values: Removed or replaced "null" entries in hospital and bed counts.

Text-to-Date Conversion: The As on column initially contained text (e.g., "As on 2017"). This was cleaned using Power Query's "Replace Values" to remove prefixes and convert it into a standard Date type.

Column Standardization: Standardized State/UT names for accurate map mapping.

📊 Dashboard Features
Statewise Concentration: A Treemap visualizing which states hold the highest number of facilities.

Bed Capacity by State: Horizontal bar chart comparing bed availability.

Urban vs Rural Ratio: A Donut chart showing the percentage split of facilities, with a central KPI for total count.

Interactive Filtering: Users can filter the entire dashboard by State or Date Range.

⚠️ Challenges & Solutions
The "Remove Errors" Trap: Initially, using "Remove Errors" on the date column deleted significant rows of data, dropping the facility count from 24K to 3K.

Solution: Reverted the step in Power Query and used Replace Values and Data Type Conversion to preserve the 24K record count.

Visual Clarity: Dark mode themes made text hard to read in some visuals.

Solution: Adjusted category labels to White/Bold and added a high-contrast Cyan theme for the donut chart and sliders.

🚀 How to Run
Clone the repository.

Open the /Scripts folder to see the Python cleaning logic.

Open the .pbix file in Power BI Desktop to interact with the dashboard.
