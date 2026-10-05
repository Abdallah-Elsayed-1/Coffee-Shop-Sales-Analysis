<div align="center">

  <h1>☕ Coffee Shop Sales Analysis Dashboard</h1>
  <p><b>An End-to-End Business Intelligence Solution built with Power BI, Power Query, DAX, and Relational Data Modeling.</b></p>

  <!-- Clean Badge Bar -->
  <p align="center">
    <code>🟡 Power BI</code> &nbsp;|&nbsp; 
    <code>🔵 Power Query & M-Code</code> &nbsp;|&nbsp; 
    <code>🟢 DAX Measures</code> &nbsp;|&nbsp; 
    <code>🟣 Star Schema Modeling</code> &nbsp;|&nbsp; 
    <code>📊 Data Cleaning (149K+ Rows)</code>
  </p>

</div>

<hr />
<br />

<h2>📌 Project Overview</h2>
<p>
  This project delivers a complete business intelligence analysis for a multi-location coffee shop chain. The project transforms raw, uncleaned transactional sales logs comprising over <b>149,000+ rows</b> into an interactive, high-impact executive dashboard using <b>Power BI</b>.
</p>
<p>
  <b>Business Objective:</b> Enable retail store decision-makers to track revenue performance, pinpoint peak operational hours, optimize staffing schedules, and uncover customer purchasing patterns across branch locations.
</p>

<br />

<h2>📊 Executive Dashboard Overview</h2>
<p>Below is the primary interactive dashboard interface featuring overall KPI metrics, product category revenue shares, and hourly transactional trends:</p>

<div align="center">
  <img src="https://i.postimg.cc/rwND4Mfj/dashbwrd.png" alt="Executive Dashboard Preview" width="100%" />
</div>

<br />
<hr />
<br />

<h2>🔑 Core Key Performance Indicators (KPIs)</h2>
<ul>
  <li><b>Total Revenue / Sales:</b> Aggregated financial earnings generated across all branches.</li>
  <li><b>Total Transactions / Orders:</b> Unique order volume processed by store registers.</li>
  <li><b>Total Quantity Sold:</b> Count of individual items and drinks fulfilled.</li>
  <li><b>Average Order Value (AOV):</b> Average revenue collected per single transaction ticket.</li>
  <li><b>Hourly Rush Patterns:</b> Analysis highlighting high-demand time slots during store operating hours.</li>
</ul>

<br />
<hr />
<br />

<h2>🛠️ Analytics Lifecycle & Technical Stages</h2>

<h3>Stage 1: Data Extraction, Cleaning & Transformation (149K+ Rows)</h3>
<p>
  The initial transactional dataset contained over <b>149,000 records</b> with data quality issues, including missing values, non-standardized timestamps, and unformatted data types.
</p>
<ul>
  <li><b>Missing Value Handling:</b> Handled null entries in transactional line items and ensured complete data integrity.</li>
  <li><b>Data Type Formatting:</b> Converted currency values, transactional times, and dates into strict data structures.</li>
  <li><b>Advanced M-Code (Power Query):</b> Applied custom conditional logic in the Advanced Editor to extract hourly blocks, day names, and custom transaction tags.</li>
</ul>

<div align="center">
  <img src="https://i.postimg.cc/dVjhCw5r/adfansyd-adytwr.png" alt="Power Query Advanced Editor M-Code" width="85%" />
</div>

<br />

<h3>Stage 2: Relational Data Modeling (Star Schema)</h3>
<p>
  Built an optimized <b>Star Schema</b> relational model by establishing clean <b>1-to-Many relationships</b> between dedicated dimension tables (<code>Dim_Calendar</code>, <code>Dim_Time</code>) and the central sales transaction table (<code>Fact_Sales</code>).
</p>
<ul>
  <li>Enabled seamless Time Intelligence filtering (Year, Month, Day of Week, Hourly Periods).</li>
  <li>Ensured fast query rendering and optimized report performance across 149k+ records.</li>
</ul>

<div align="center">
  <img src="https://i.postimg.cc/g2HxhmgB/mwdylynj.png" alt="Star Schema Data Model" width="85%" />
</div>

<br />

<h3>Stage 3: DAX Measure Hierarchy & Calculations</h3>
<p>
  Constructed a dedicated Measure Table containing calculated DAX expressions for business KPIs:
</p>
<ul>
  <li><code>Total Sales</code> = <code>SUM(Fact_Sales[transaction_qty] * Fact_Sales[unit_price])</code></li>
  <li><code>Total Orders</code> = <code>DISTINCTCOUNT(Fact_Sales[transaction_id])</code></li>
  <li><code>Average Order Value</code> = <code>DIVIDE([Total Sales], [Total Orders], 0)</code></li>
</ul>

<div align="center">
  <img src="https://i.postimg.cc/Jz5sXMpn/kpis.png" alt="DAX Measures Table" width="75%" />
</div>

<br />
<hr />
<br />

<h2>🎯 Dynamic Slicing & Dashboard Interactivity</h2>
<p>
  The report provides deep interactivity, allowing store managers to slice data dynamically by peak hours or store branches:
</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>1. Filtering by Hourly Peak Demand</h4>
        <img src="https://i.postimg.cc/13r8FsvC/fltr-balsa-h.png" width="95%" alt="Filtered by Hour" />
        <p align="left"><small>Isolates sales metrics during specific rush hours to adjust kitchen and barista staffing levels.</small></p>
      </td>
      <td width="50%" align="center" valign="top">
        <h4>2. Filtering by Store Location</h4>
        <img src="https://i.postimg.cc/rwND4MfZ/fltr-b-allwkysn.png" width="95%" alt="Filtered by Branch Location" />
        <p align="left"><small>Drills down into individual branch performance (e.g., Astoria, Hell's Kitchen, Lower Manhattan).</small></p>
      </td>
    </tr>
  </table>
</div>

<br />
<hr />
<br />

<h2>💡 Strategic Recommendations & Insights</h2>
<ol>
  <li><b>Staff Scheduling Optimization:</b> Shift additional store personnel to high-volume morning hours (7:00 AM – 10:00 AM) to reduce order queue times.</li>
  <li><b>AOV Enhancement Strategies:</b> Implement cross-selling bundles (e.g., pairing high-margin coffee drinks with slow-moving bakery products).</li>
  <li><b>Location Inventory Allocation:</b> Align inventory replenishment cycles with top-selling branches to prevent stockouts during peak days.</li>
</ol>

<br />
<hr />
<br />

<h2>📂 Repository Architecture</h2>
<pre>
├── Data/                        # Raw transactional dataset (149k+ records)
├── Reports/                     # Coffee_Shop_Sales_Analysis.pbix
├── Screenshots/                 # Process and dashboard visual assets
└── README.md                    # Project documentation
</pre>
