# Developing and Maintaining $1.1M CAD Wireless Network Solutions for 2 Enterprise Clients (100% Retention Rate)
## Project Summary
<a href="https://www.ligaccuver.com/pages/eng/main.asp"> <img width="221" height="27" alt="LIG Accuver" src="https://github.com/user-attachments/assets/c31a1ad4-b9f9-4e4e-bb35-cb0c0703760c" /> </a>

From 2023 to 2025, I served as the sole **Full-Stack engineer** at **LIG Accuver**, developing and maintaining customized solutions for **3 major on-premise client projects totalling $1.1M CAD/year.** 

The clients were 2 leading mobile carriers in Korea:  
- **SK Telecom** (approximately **$16.6B CAD** in 2025 annual revenue)
- **KT Corporation** (approximately **$27.5B CAD** in 2025 annual revenue)

Both first became LIG Accuver clients in 2020.

| Metric           | Impact                                                     |
| ---------------- | ---------------------------------------------------------- |
| **$1.1M / year** | Recurring yearly revenue from projects                     |
| **2 + years**    | Project lengths, with 0 complaints and 100% retention rate |


## Background
[LIG Accuver](https://www.ligaccuver.com/pages/eng/main.asp) is wireless network testing and analysis company that generated approximately **$186M CAD in revenue in 2025.** It provides software solutions to major mobile carriers in Korea, North America and Europe used for measuring, analyzing, and visualizing mobile network performance. 

XCAP is one of LIG Accuver’s most popular software solutions. 

It is a web or cloud-based post-processing system that helps telecom engineers analyze wireless network data, visualize test results, and troubleshoot network failures through charts, maps, tables, reports, and detailed log analyses.

<a href="https://www.ligaccuver.com/pages/eng/product_view.asp?sPCate=1&sGCate=7&sPSeq=18"> <img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/29cebb3f-82dc-4129-9d3e-cc8103958cde" /></a>

<p align="center"> <a href="https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT"><strong>Demo Video of XCAP-Cloud</strong></a> </p>

## My Role / Responsibilities 

My main responsibility was developing and maintaining the data visualization modules for large-scale wireless network datasets, with the goal of providing high-quality personalized solutions that keep SK Telecom and KT coporation as ongoing LIG Accuver clients.


## Tech Stack

| Stack                    | Summary                                                                                                                                                                              |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Javacscipt / Vue**     | Developed GUI-based query builder and data visualization features, allowing users to create, modify, and execute analysis queries without manually writing complex query statements. |
| **Java / Spring boot**   | Built backend APIs for managing users, project settings, query metadata, and analysis result delivery.                                                                               |
| **PostgreSQL / MyBatis** | Stored and retrieved metadata such as user information, query configurations, and visualization settings.                                                                            |
| **AgGrid / HighChart**     | Implemented interactive tables, charts, and graphs to visualize large-scale wireless network analysis results returned from the internal XDB system.                                 |


## System Context
<img width="1448" height="1086" alt="XCAP architecture" src="https://github.com/user-attachments/assets/6811d7f9-b651-4482-a41f-4f9ca7556e70" />

The system used a Vue.js frontend, a Spring Boot backend, PostgreSQL for metadata management, and an internal XDB system for large-scale wireless network data analysis.

Users created and modified analysis queries through the Vue-based GUI. The Spring Boot backend managed user information, project settings, query metadata, and visualization settings in PostgreSQL. When users executed a query, the backend sent the generated query to the company’s internal XDB system, which processed large-scale wireless network datasets and returned the analysis results. The frontend then visualized those results through interactive charts, graphs, and tables.


## Key Features
<a href="https://www.ligaccuver.com/pages/eng/product_view.asp?sPCate=1&sGCate=7&sPSeq=18"> <img width="1168" height="319" alt="image" src="https://github.com/user-attachments/assets/3e78ebae-e924-4dc6-9777-993dc6b02e58" /></a>

<p align="center">
  <b>Dashboard</b> - Main Dashboard Showing Graphs and Charts &nbsp;&nbsp;|&nbsp;&nbsp;
  <b>AI Analysis</b> - Customizable Spreadsheets for drill-down
</p>

XCAP can analyze and showcase mobile carrier data through a variety of methods. 

I was primarily responsible for developing and improving these two core XCAP features: the Dashboard and AI Analysis / GUI Query Builder.

### Dashboard
- The Dashboard feature turns large amounts of mobile network measurement data into interactive charts and graphs. I worked on features that helped telecom engineers monitor key metrics, compare test results, and identify abnormal patterns without manually extracting raw data.
- The queried results were then visualized through interactive charts and graphs, helping telecom engineers analyze network performance trends, compare test results, and identify abnormal patterns more efficiently. This reduced the need for manual data extraction and made complex network data easier to understand for both technical and non-technical users.
- Users can save dashboard presets with conditions such as data collection period, target datasets, chart types, and visualization settings. These presets can be reused for repeated analysis, reducing repeated setup work and making frequently used analysis views easier to manage.

### AI Analysis(GUI Query Builder)
* The AI Analysis feature allows users to investigate selected mobile network issues in more detail after identifying trends on the Dashboard. It queries pre-processed AI data so engineers can focus on more relevant and filtered measurement results.
* Users can apply advanced query options such as filters, grouping conditions, and calculation rules through a GUI-based interface, instead of manually writing complex SQL queries.
* The queried results can be reviewed in tables and exported as CSV files or images for reporting, helping engineers move from high-level monitoring to detailed analysis and documentation.
* This made deeper network data exploration more accessible and reduced the need for manual query writing, repeated data extraction, and developer support.

## Development & Maintainance Highlights
- Worked closely for **2 years** with the client-facing lead who managed direct communication with both enterprise clients, **helping maintain zero client complaints through clear documentation, fast issue resolution, and reliable delivery**.
- Delivered **15 major/customized features across 210 tickets** from 2023 to 2025, covering GUI query building, SaaS integration, and SMAP AI customization.
- Reduced major legacy code areas by **60–75%**, including **4,000 → 1,000 lines**, **3,000 → 1,000 lines**, and **1,000 → 300 lines** refactors.
- Reduced follow-up revision requests by approximately **80%**, from **3–4 per feature to 0–1**, through clearer documentation and implementation alignment.
- Maintained **zero client complaints** and reduced meeting time from **1.5–2 hours to 30 minutes–1 hour** through clear client-facing communication.
- Built GUI-based query workflows that allowed users to create, edit, save, validate, and run complex data queries without manually writing query statements.
- Customized Ag-Grid, Highcharts, Split.js, and drag-and-drop UI behavior under legacy dependency constraints.
- Restored stable SaaS behavior for **5 legacy on-premise API integrations** and centralized scattered integration logic into maintainable modules.
- Created **3 internal wiki documents** covering **15 cross-team integration issues**, including design intent, change history, and tagged commits.

## Actions
### May 2023: Fast Legacy Cleanup and Debugging
* My first action was cleaning legacy code by **improving readability, removing duplication**, and handling basic debugging tasks. I completed **8 debugging and legacy cleanup tasks, each within one day**. 
	- **Improved 30+ inconsistent multi-language buttons and labels**, such as OK, Yes, and No, by organizing repeated UI text into reusable shared modules, **reducing related code by 60% from 240 lines to 96 lines**.
	- **Removed 200 redundant lines** from a cross-team integration while preserving functionality.

### Jun 2023 to Dec 2023: 5 Major Features / Building the Core GUI Query Builder
* The next request was to add **5 major features(80 tickets)** that **allowed users to create, edit, and run custom data queries through a GUI-based interface**, without needing to manually write complex query statements.
    - Reworked a **4,000-line legacy page** into 7 reusable modules, **reducing it to approximately 1,000 lines**. 
    - **Implemented drag-and-drop field selection, resizable split-pane layouts, and filter-condition builders to help users configure complex queries through the UI.**
	    - Integrated **Split.js, Ag-Grid, and drag-and-drop UI libraries** while resolving layout and interaction conflicts between third-party components.
    - Designed a complex data-query workflow with an Excel pivot-table-like user experience, helping users analyze data without manually writing complex query statements.
    - **Improved code readability and maintainability** by **clarifying variable names**, simplifying functions, **adding JSDoc** comments, and applying shared **ESLint and Prettier standards**.
    - **Completed all first-phase requirements** for the initial 2023 demo.
    
### Jan 2024 to July 2024 - 4 Major Features / Advanced UI Features, Presets, and Ag-Grid Workarounds
* **Completed 4 features**(50 tickets) as advanced enhancements for the GUI-based Query builder, **including UI customization, preset save/load, and preset validation**.
* Developed unsupported UI behaviors through custom Ag-Grid workarounds after investigating **30,000+ lines of open source code**.
- **Eliminated a manual restart step** **by adding preset error-detection logic** that alerted users when saved configurations no longer matched modified tables.
- **Improve readability and maintainability by** **refactoring** semi-hard-coded configuration logic from **3,000 lines to 1,000 lines** by separating reusable modules and shared constants.

### From Jul to Dec 2024: 3 Major Features / SaaS Migration Support and Cross-Team API Stabilization
- Refactored legacy on-premise API integrations for **5 existing XCAP features/modules**, restoring stable behavior for the cloud-based SaaS version.
- Reduced scattered integration logic from **1,000 lines to 300 lines** by centralizing it into a single module **for easier updates and debugging**.
- Reduced follow-up revision requests from **4 per feature to 0–1** by creating **3 internal wiki documents** covering **15 cross-team integration issues**, design intent, change history, and tagged commits.
- **Stabilized cross-team API integrations** by resolving undocumented parameters, table changes, and legacy compatibility issues.
 
### From Aug 2024 to Jul 2025: 6 Major Features / Customizing Features for Client with $16.6B CAD Annual Revenue in 2025
- Completed **80 tickets** to customize existing XCAP features and develop **6 new SMAP AI features** for SK Telecom(approximately **$16.6B CAD** in 2025 annual revenue).
- Built Ag-Grid and Highcharts-based visualization features by customizing queries across **4–6 big-data tables** without JOIN support, allowing users to view accurate mobile network measurement insights.
- Reduced follow-up revision requests by approximately **80%**, from **3–4 per feature to 0–1**, by documenting feature behavior, edge cases, and design intent.
- Maintained **zero client complaints**, reduced meeting time from **1.5–2 hours to 30 minutes–1 hour**, and **cut follow-up revision requests by** approximately **80%** through clear feature documentation and client-facing communication.


## Results

| Metric           | Impact                                                     |
| ---------------- | ---------------------------------------------------------- |
| **$1.1M / year** | Recurring yearly revenue from projects                     |
| **2 + years**    | Project lengths, with 0 complaints and 100% retention rate |

## ENGINEERING SKILLS IMPROVED
- Improved maintainability in a legacy Vue.js codebase while continuing to deliver new features.
    - Designed lightweight state-management patterns without Vuex by using Vue components, shared logic, and structured data flow.
    - Refactored legacy code across multiple pull requests by removing duplication, simplifying complex logic, and separating responsibilities more clearly.
    - Reduced code volume while expanding functionality, making the codebase easier to understand and maintain.
- Delivered required UI features under strict technical constraints.
    - Built a GUI-based query builder using an older free version of Ag-Grid, as upgrading the library was not allowed by project requirements.
    - Analyzed Ag-Grid’s internal behavior and implemented custom workarounds for table interactions not supported by the documented API.
    - Learned the importance of separating business logic from UI library dependencies, documenting trade-offs, and designing maintainable abstraction layers.


<p align="center"> <a href="https://github.com/Magpie1000/"> <img src="https://img.shields.io/badge/←%20Back%20to%20Main-24292f?style=for-the-badge" alt="Back to Main" /> </a> </p>
