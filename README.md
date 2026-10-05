<p align="center">
  <b>Tech Stack & Tools:</b>&nbsp; 
  <code>🟡 Power BI</code> &nbsp;|&nbsp; 
  <code>🔵 Power Query</code> &nbsp;|&nbsp; 
  <code>🟢 DAX Measures</code> &nbsp;|&nbsp; 
  <code>🟣 Star Schema Modeling</code>
</p>

<h2>📌 Project Overview</h2>
<p>
  This project provides a comprehensive analysis of sales performance for a multi-location coffee shop chain. The goal is to transform raw transactional sales data into actionable business insights using <b>Power BI</b>, enabling store managers to optimize inventory, staff scheduling, and product offerings based on peak sales hours and product popularity.
</p>

<br />

<h2>📊 Executive Dashboard Preview</h2>
<div align="center">
  <img src="https://i.postimg.cc/rwND4Mfj/dashbwrd.png" alt="Coffee Shop Sales Main Dashboard" width="100%" />
</div>

<br />
<hr />
<br />

<h2>🔑 Key Performance Indicators (KPIs) & Business Insights</h2>
<ul>
  <li><b>Total Revenue / Sales:</b> Overall earnings calculated across all operating locations.</li>
  <li><b>Total Quantity Sold:</b> Volume of products delivered to customers.</li>
  <li><b>Total Orders:</b> Count of unique sales transactions.</li>
  <li><b>Average Order Value (AOV):</b> Revenue generated per single customer order.</li>
  <li><b>Peak Sales Hours Analysis:</b> Identifies high-demand periods during the day (e.g., morning coffee rushes) to align staffing and operational efficiency.</li>
  <li><b>Multi-Location Performance:</b> Dynamic filtering by store locations to compare top-performing branches.</li>
</ul>

<br />
<hr />
<br />

<h2>🛠️ Data Architecture & Modeling</h2>

<h3>1. Advanced ETL & Transformation (Power Query)</h3>
<p>
  Cleaned raw transactional datasets, adjusted column types, and created custom date/time conditional attributes. Applied M-code transformations in Advanced Editor to optimize query performance.
</p>

<div align="center">
  <img src="https://i.postimg.cc/dVjhCw5r/adfansyd-adytwr.png" alt="Power Query Advanced Editor" width="85%" />
</div>

<br />

<h3>2. Relational Data Model (Star Schema)</h3>
<p>
  Established a clean <b>1-to-Many relationship</b> between dedicated Calendar and Time dimension tables and the Sales Fact Table. Enabled Time Intelligence calculations and dynamic slicing across years, months, days, and hours.
</p>

<div align="center">
  <img src="https://i.postimg.cc/g2HxhmgB/mwdylynj.png" alt="Data Model Relationships" width="85%" />
</div>

<br />

<h3>3. DAX Calculations</h3>
<p>
  A dedicated Measure Table was constructed using DAX formulas for accurate KPI calculations including Total Sales, Total Orders, Total Quantity, and Average Order Value.
</p>

<div align="center">
  <img src="https://i.postimg.cc/Jz5sXMpn/kpis.png" alt="DAX Measures Table" width="75%" />
</div>

<br />
<hr />
<br />

<h2>🎯 Dashboard Features & Interactivity</h2>

<p>The dashboard includes dynamic time slicers (Month, Day of Week, Hour of Day) and location drill-downs.</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>Hourly Peak Filtering</h4>
        <img src="https://i.postimg.cc/13r8FsvC/fltr-balsa-h.png" width="95%" />
      </td>
      <td width="50%" align="center" valign="top">
        <h4>Branch Location Filtering</h4>
        <img src="https://i.postimg.cc/rwND4MfZ/fltr-b-allwkysn.png" width="95%" />
      </td>
    </tr>
  </table>
</div>

<br />
<hr />
<br />

<h2>💡 Key Business Recommendations</h2>
<ol>
  <li><b>Staff Optimization:</b> Increase staff during identified peak morning hours to minimize customer wait times and prevent sales bottlenecks.</li>
  <li><b>Product Bundling:</b> Promote top-selling beverage items alongside slow-moving bakery items during off-peak hours to raise Average Order Value (AOV).</li>
  <li><b>Inventory Management:</b> Ensure inventory restocking aligns with high-volume branches and high-demand days of the week.</li>
</ol>

<br />
<hr />
<br />

<h2>📂 Project Repository Structure</h2>
<pre>
├── Data/                       # Raw sales CSV/Excel files
├── Reports/                    # Coffee_Shop_Sales_Analysis.pbix
├── Screenshots/                # Dashboard visual assets
└── README.md                   # Project documentation
</pre>
