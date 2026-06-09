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

[Demo Video of XCAP-Cloud](https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT)

## My Role / Responsibilities 

My main responsibility was developing and maintaining the data visualization modules for large-scale wireless network datasets, with the goal of providing high-quality personalized solutions that keep SK Telecom and KT coporation as ongoing LIG Accuver clients.
<a href="https://www.ligaccuver.com/pages/eng/product_view.asp?sPCate=1&sGCate=7&sPSeq=18"> <img width="1168" height="319" alt="image" src="https://github.com/user-attachments/assets/3e78ebae-e924-4dc6-9777-993dc6b02e58" /></a>

### Dashboard

The Dashboard feature allows users to save, manage, and monitor measurement data through various chart types. Users can configure dashboard presets, including conditions such as data collection period, target datasets, and visualization settings, then reuse those presets for repeated analysis.

This makes it easier for engineers to track key network metrics, compare measurement results, and manage frequently used analysis views without rebuilding the same charts manually.

### AI Analysis

The AI Analysis feature provides a pivot-table-like query interface that allows users to create analysis queries more easily. Instead of manually writing complex SQL, users can select fields, define grouping conditions, apply aggregate functions, and organize analysis results through a GUI-based interface.

This feature helps users generate custom statistical analysis queries more efficiently and makes large-scale network data exploration more accessible to engineers who may not be comfortable writing SQL directly.


## Tech Stack

| Stack                    | Summary                                                                                                                                                                              |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Javacscipt / Vue**     | Developed GUI-based query builder and data visualization features, allowing users to create, modify, and execute analysis queries without manually writing complex query statements. |
| **Java / Spring boot**   | Built backend APIs for managing users, project settings, query metadata, and analysis result delivery.                                                                               |
| **PostgreSQL / MyBatis** | Stored and retrieved metadata such as user information, query configurations, and visualization settings.                                                                            |
| **AgGrid / HiChart**     | Implemented interactive tables, charts, and graphs to visualize large-scale wireless network analysis results returned from the internal XDB system.                                 |


## System Context
<img width="1448" height="1086" alt="XCAP architecture" src="https://github.com/user-attachments/assets/6811d7f9-b651-4482-a41f-4f9ca7556e70" />

The system used a Vue.js frontend, a Spring Boot backend, PostgreSQL for metadata management, and an internal XDB system for large-scale wireless network data analysis.

Users created and modified analysis queries through the Vue-based GUI. The Spring Boot backend managed user information, project settings, query metadata, and visualization settings in PostgreSQL. When users executed a query, the backend sent the generated query to the company’s internal XDB system, which processed large-scale wireless network datasets and returned the analysis results. The frontend then visualized those results through interactive charts, graphs, and tables.


## Actions
### Development Highlights 

More coming...
> Memo to Grant -> I need to look up to the code that i worked - which is saved in my old computer. I fixed it but still need little bit more time to finish up. 

### Maintenance and Optimization Highlights

> Memo to Grant -> I need to look up to the code that i worked - which is saved in my old computer. I fixed it but still need little bit more time to finish up. 
## Results

| Metric                         | Result                      | Impact                                                                                                         |
| ------------------------------ | --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **$1.1M / year**               | **Revenue**                 | served as sole full-stack developer for 3 projects of $1.1M CAD/year for 2 leading mobile carriers in Korea    |
| **2 + years**                  | **0 complaints**            | Handeled 3 projects for 2 years without any complaints.                                                        |
| **100% Client retention rate** | **2 Major mobile carieers** | Acieved 100% client retention rate with successfully developing and maintaining 3 projects with no complaints. |

## Takewaways
- Improved maintainability in a legacy Vue.js codebase while continuing to deliver new features.
    - Designed lightweight state-management patterns without Vuex by using Vue components, shared logic, and structured data flow.
    - Refactored legacy code across multiple pull requests by removing duplication, simplifying complex logic, and separating responsibilities more clearly.
    - Reduced code volume while expanding functionality, making the codebase easier to understand and maintain.
- Delivered required UI features under strict technical constraints.
    - Built a GUI-based query builder using an older free version of Ag-Grid, as upgrading the library was not allowed by project requirements.
    - Analyzed Ag-Grid’s internal behavior and implemented custom workarounds for table interactions not supported by the documented API.
    - Learned the importance of separating business logic from UI library dependencies, documenting trade-offs, and designing maintainable abstraction layers.

