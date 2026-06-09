# Building and Maintaining 4 Big-data monitoring software for 
## Project summary
Served as Full-Stack engineer in LIG Accuver, 3 major on-premise client projects ($1.1M CAD/year), developing and maintaining customized solutions for 2 leading mobile carriers in Korea. 

| Metric                         | Result                      | Impact                                                                                                         |
| ------------------------------ | --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **$1.1M / year**               | **Revenue**                 | served as sole full-stack developer for 3 projects of $1.1M CAD/year for 2 leading mobile carriers in Korea    |
| **2 + years**                  | **0 complaints**            | Handeled 3 projects for 2 years without any complaints.                                                        |
| **100% Client retention rate** | **2 Major mobile carieers** | Acieved 100% client retention rate with successfully developing and maintaining 3 projects with no complaints. |

## Background
[LIG Accuver](https://www.ligaccuver.com/pages/eng/main.asp) is wireless network testing and analysis company that generated approximately CAD 186 million in revenue in 2025. It provides software solutions to major mobile carieers in Korea, North America and Europe, for measuring, analyzing, and visualizing mobile network performance. 

**XCAP / XCAP-Cloud** was the project platform I worked on at LIG Accuver. It is a web-based post-processing system that helps telecom engineers analyze wireless network measurement data, visualize test results, and troubleshoot network failures through charts, maps, tables, reports, and detailed log analysis.
<img width="3259" height="2475" alt="image" src="https://github.com/user-attachments/assets/29cebb3f-82dc-4129-9d3e-cc8103958cde" />

[Demo Video of XCAP-Cloud](https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT)

## My Role / Responsibilities 

My main responsibility in XCAP / XCAP-Cloud was developing and maintaining the data visualization module for large-scale wireless network datasets. I built features that allowed users to create, edit, and run custom data queries through a GUI-based interface, without needing to manually write complex query statements.

The queried results were then visualized through interactive charts and graphs, helping telecom engineers analyze network performance trends, compare test results, and identify abnormal patterns more efficiently. This reduced the need for manual data extraction and made complex network data easier to understand for both technical and non-technical users.

<img width="1696" height="947" alt="image" src="https://github.com/user-attachments/assets/2da3a839-ac82-47be-b552-c585e6ce1425" />



## Tech stack

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


## Action
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

