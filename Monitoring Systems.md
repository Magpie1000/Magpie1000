# Building a SaaS-Ready Monitoring System for LIG Accuver($186M CAD Revenue in 2025)
## Project Summary
<a href="https://www.ligaccuver.com/pages/eng/main.asp"> <img width="221" height="27" alt="LIG Accuver" src="https://github.com/user-attachments/assets/c31a1ad4-b9f9-4e4e-bb35-cb0c0703760c" /> </a> 

From 2023 to 2024, I served as a DevOps / Cloud Monitoring engineer in a **LIG Accuver's company-wide task force** to prepare XCAP for **SaaS and cloud-based deployment**.

| Metric                                                               | Impact                                                                                                                                                                                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **33% AWS cost reduction**                                           | Used Kubecost to identify Kubernetes resource usage and cost optimization opportunities, helping reduce unnecessary AWS spending for the XCAP-Cloud EKS environment.                                                     |
| **$1.8M CAD projects reviewd Monitoring system for operational use** | Built an observability system that was reviewed as the monitoring foundation for projects worth approximately CAD 1.8M, covering performance monitoring, log monitoring, cost visibility, and troubleshooting workflows. |
| **5 internal seminars including demos and hands-on session**         | Helped System Engineers, Cloud Task Force, and other teams understand how to use the monitoring stack for troubleshooting and operation.                                                                                 |
| **6 A-to-Z technical guides**                                        | Reduced onboarding friction by documenting monitoring setup, dashboard usage, log investigation, and operational workflows.                                                                                              |

## Background

[**LIG Accuver**](https://www.ligaccuver.com/pages/eng/main.asp) is wireless network testing and analysis company that generated approximately **$186M CAD in revenue in 2025.** It provides software solutions to major mobile carriers in Korea, North America and Europe used for measuring, analyzing, and visualizing mobile network performance. 

XCAP is one of LIG Accuver’s most popular software solutions. 

It is a web or cloud-based post-processing system that helps telecom engineers analyze wireless network data, visualize test results, and troubleshoot network failures through charts, maps, tables, reports, and detailed log analyses.

**The goal** of the task force was to make the **existing XCAP-Cloud platform deployable across multiple infrastructure environments**, including **AWS EKS, on-premise Kubernetes, Docker-based deployments, and EC2**. 

<a href="https://www.ligaccuver.com/pages/eng/product_view.asp?sPCate=1&sGCate=7&sPSeq=18"> <img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/29cebb3f-82dc-4129-9d3e-cc8103958cde" /></a>

<p align="center"> <a href="https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT"><strong>Demo Video of XCAP-Cloud</strong></a> </p>

## My Role / Responsibilities
My main responsibility was to build a monitoring system for XCAP-Cloud across four deployment environments: AWS EKS, on-premise Kubernetes, Docker, and EC2.

I designed and configured monitoring components to collect infrastructure metrics, application metrics, container status, logs, and resource usage data. The monitoring system helped developers and operators understand whether the platform was running correctly, identify failures more quickly, and compare operational behavior across different deployment environments.

## Tech Stack

| Stack                           | Summary                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **AWS EKS**                     | Supported cloud-native deployment and monitoring for XCAP-Cloud on managed Kubernetes infrastructure.                |
| **On-premise Kubernetes(RKE2)** | Built monitoring support for Kubernetes clusters running in customer-controlled or internal on-premise environments. |
| **Docker / EC2**                | Supported containerized and VM-based deployment cases outside Kubernetes environments.                               |
| **Prometheus**                  | Collected infrastructure, container, and application metrics across different deployment environments.               |
| **Grafana**                     | Built dashboards to visualize system health, resource usage, application status, and operational metrics.            |
| **Loki**                        | Collected and queried application and system logs for troubleshooting.                                               |
| **Helm**                        | Managed Kubernetes monitoring components through reusable and configurable chart values.                             |
| **ArgoCD**                      | Supported GitOps-based deployment and synchronization of monitoring components.                                      |
| **Kubecost**                    | Helped monitor Kubernetes resource usage and cloud cost visibility for EKS-based environments.                       |


## Development & Maintenance Highlights

* Built a SaaS-ready observability system across **4 major deployment environments**: **AWS EKS**, on-premise **Kubernetes**, **Docker-based servers**, and **EC2**.
* Implemented metric, log, and cost monitoring workflows using **Prometheus, Grafana, Loki, Kubecost, Helm, and docker-compose**.
* Supported **33% AWS cost reduction** by using Kubecost to identify Kubernetes resource usage and cost optimization opportunities.
* Delivered **5 internal seminars** with demos and hands-on explanations for System Engineers, Cloud TF members, and related teams.
* Created **6 A-to-Z technical guides** covering monitoring setup, dashboard usage, log investigation, performance analysis, alert configuration, Kubecost, and AWS EBS metrics.

## Actions
### Q1 2024 — Compared 3 Monitoring Stacks and Delivered 3 Technical Presentations

* Compared **3 monitoring stack options** — ELK/EFK, PLG, and AWS CloudWatch — and delivered **3 technical presentations** to support Cloud TF stack selection.
* Evaluated each option across **8 criteria**: metrics, logs, dashboards, alerts, scalability, operational complexity, documentation quality, and cost.
* Recommended **PLG** as the main monitoring direction after identifying **25–70% potential cost savings** compared with EFK, along with cloud-native architecture, Helm-based setup, horizontal scalability, and unified metric/log monitoring.
    * Researched AWS CloudWatch as a managed alternative, covering **7 AWS services/features** — Container Insights, Logs, SNS, Lambda, EventBridge, dashboards, and alerts — with an estimated monthly cost of approximately **$150**.

##### 여기에 프레젠테이션 사진 추가

### Q2 2024 — Built 1 PLG Prototype, Validated 4 Workflows, Delivered 2 Hands-On Sessions
* Built the first working **Docker-compose PLG monitoring prototype** and deployed it to **2 internal test servers** for validation.
* Reduced manual troubleshooting work for the System Engineering team by **replacing direct server log inspection** **with Grafana/Loki-based log search, filtering, and dashboard workflows**.
  * Proved the prototype across **4 core workflows**: metric collection, log collection, dashboard access, and troubleshooting.
* Delivered **2 hands-on usage guide sessions** for Cloud TF and System Engineering, helping other teams test the prototype and learn Grafana/Loki-based monitoring workflows.
    * Collected **2 weeks of user feedback** and improved dashboard usability, documentation, and troubleshooting guidance.

##### 여기에 프레젠테이션 사진 추가

### Q3 2024 — Expanded PLG Monitoring Across 4 Environment Types and Validated 12 Test Runs Without Unexpected AWS Cost Issues

* **Deployed and stabilized** PLG monitoring across **AWS EKS, EC2, on-premise RKE2, and 4 internal servers** without unexpected AWS cost issues.
* **Validated Docker-based monitoring** through **12 load/performance test runs** on **4 on-premise 256GB RAM servers**, including **two-day weekend testing sessions**.
* Applied **5 feedback-based usability improvements** from the Q2 prototype review.
* Created **2 practical usage manuals** and delivered **2 architecture guide sessions** covering Docker-based and Kubernetes-based monitoring models.
* Standardized Helm chart versions and environment-specific settings to improve deployment consistency and reduce installation issues.

##### 여기에 프레젠테이션 사진 추가

### Q4 2024 — Automated Grafana Setup, Removed 1 Developer Standby, and Reduced AWS Costs by 33%
* Automated Grafana initial setup, eliminating **1 developer standby requirement** during late-night installations and saving approximately **2 hours per setup** through automated user creation, dashboard provisioning, and configuration.
* Reduced AWS costs by **33%**, from approximately **$990 to $660**, by installing and operating **Kubecost** for Kubernetes cost visibility.
* Delivered **2 additional hands-on sessions** to help engineers use Grafana dashboards, investigate logs, and follow monitoring workflows.
* Reduced Helm chart configuration YAML from approximately **200 lines to 65 lines** by simplifying values and removing unnecessary settings.
* Created **6 A-to-Z monitoring manuals** and documented **4 troubleshooting cases** for future maintenance.
* Migrated and upgraded Kubernetes monitoring Helm charts to improve availability, stability, scalability, and multi-cluster readiness.


##### 여기에 프레젠테이션 사진 추가


https://docs.google.com/presentation/d/1nV7nl2ik3LvQdGOb05OGBLeqbxMuGhPVFgi4tUe-0XY/edit?usp=sharing

https://docs.google.com/presentation/d/1qDeYAhviwo_KtIIOGKnNgqAm_ps_gTjju8yCiThxF9g/edit?usp=sharing

https://docs.google.com/presentation/d/1hXU2GqlQA9wcMu_3B68KOMODap8HBsRyI53MrW25J2I/edit?usp=sharing


<img width="1468" height="676" alt="image" src="https://github.com/user-attachments/assets/b7afe9b7-3da9-4021-95ab-1ef294d82e23" />




## Result

| Metric                                                               | Impact                                                                                                                                                                                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **33% AWS cost reduction**                                           | Used Kubecost to identify Kubernetes resource usage and cost optimization opportunities, helping reduce unnecessary AWS spending for the XCAP-Cloud EKS environment.                                                     |
| **$1.8M CAD projects reviewd Monitoring system for operational use** | Built an observability system that was reviewed as the monitoring foundation for projects worth approximately CAD 1.8M, covering performance monitoring, log monitoring, cost visibility, and troubleshooting workflows. |
| **5 internal seminars including demos and hands-on session**         | Helped System Engineers, Cloud Task Force, and other teams understand how to use the monitoring stack for troubleshooting and operation.                                                                                 |
| **6 A-to-Z technical guides**                                        | Reduced onboarding friction by documenting monitoring setup, dashboard usage, log investigation, and operational workflows.                                                                                              |

## Takeaways

- Learned how to design observability for real production systems across different infrastructure environments.
    - Built monitoring support for AWS EKS, on-premise Kubernetes, Docker, and EC2 deployment cases.
    - Understood how infrastructure differences affect monitoring design, deployment strategy, and troubleshooting workflows.
    - Learned to think beyond application development and consider system health, operational visibility, and maintainability.
        
- Strengthened cloud-native and DevOps engineering skills through a company-wide SaaS transition project.
    - Worked with Kubernetes, Helm, ArgoCD, Prometheus, Grafana, Loki, and AWS EKS.
    - Designed reusable monitoring configurations that could be adapted to multiple environments.
    - Learned the importance of standardizing observability when moving from customized on-premise projects to scalable cloud-based delivery.

<p align="center"> <a href="https://github.com/Magpie1000/"> <img src="https://img.shields.io/badge/←%20Back%20to%20Main-24292f?style=for-the-badge" alt="Back to Main" /> </a> </p>
