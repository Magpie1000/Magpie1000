# Building a SaaS-Ready Monitoring System for LIG Accuver ($186M CAD Revenue in 2025)
## Project Summary
<a href="https://www.ligaccuver.com/pages/eng/main.asp"> <img width="221" height="27" alt="LIG Accuver" src="https://github.com/user-attachments/assets/c31a1ad4-b9f9-4e4e-bb35-cb0c0703760c" /> </a> 

From 2023 to 2024, I served as a DevOps / Cloud Monitoring engineer in a **LIG Accuver's company-wide Cloud Task Force** to prepare XCAP for **SaaS and cloud-based deployment**.

The Cloud Task Force consisted of 12 LIG Accuver members across Frontend Engineer, Backend Engineer, DevOps engineer, and System Engineer. 

The goal of the task force was to make the existing XCAP-Cloud platform deployable across multiple infrastructure environments, including AWS EKS, on-premise Kubernetes, Docker-based deployments, and EC2.

At the beginning of this project, XCAP-Cloud was only deployable using on-premise services. This severely limited XCAP-Cloud’s growth, because on-premise services required significantly more time and LIG Accuver employees physically traveling to the client site. 

Making XCAP-Cloud deployable across varied infrastructures would both reduce the onboarding time for all new users, and allow LIG Accuver to acquire customers anywhere in the world.  


| Metric                                                               | Impact                                                                                                                                                                                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **33% AWS cost reduction**                                           | Used Kubecost to identify Kubernetes resource usage and cost optimization opportunities, helping reduce unnecessary AWS spending for the XCAP-Cloud EKS environment.                                                     |
| **$1.8M CAD projects reviewed Monitoring system for operational use** | Built an observability system that was reviewed as the monitoring foundation for projects worth approximately CAD 1.8M, covering performance monitoring, log monitoring, cost visibility, and troubleshooting workflows. |
| **5 internal seminars including demos and hands-on session**         | Helped System Engineers, Cloud Task Force, and other teams understand how to use the monitoring stack for troubleshooting and operation.                                                                                 |
| **6 A-to-Z technical guides**                                        | Reduced onboarding friction by documenting monitoring setup, dashboard usage, log investigation, and operational workflows.                                                                                              |

## Background

[**LIG Accuver**](https://www.ligaccuver.com/pages/eng/main.asp) is a wireless network testing and analysis company that generated approximately **$186M CAD in revenue in 2025.** It provides software solutions to major mobile carriers in Korea, North America and Europe used for measuring, analyzing, and visualizing mobile network performance. 

XCAP is one of LIG Accuver’s most popular software solutions. 

It is a web or cloud-based post-processing system that helps telecom engineers analyze wireless network data, visualize test results, and troubleshoot network failures through charts, maps, tables, reports, and detailed log analyses.

**The goal** of the **Cloud Task Force** was to make the **existing XCAP-Cloud platform deployable across multiple infrastructure environments**, including **AWS EKS, on-premises Kubernetes, Docker-based deployments, and EC2**. 

<a href="https://www.ligaccuver.com/pages/eng/product_view.asp?sPCate=1&sGCate=7&sPSeq=18"> <img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/29cebb3f-82dc-4129-9d3e-cc8103958cde" /></a>

<p align="center"> <a href="https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT"><strong>Demo Video of XCAP-Cloud</strong></a> </p>

## My Role / Responsibilities
My main responsibility was to build a monitoring system for XCAP-Cloud across four deployment environments: AWS EKS, on-premises Kubernetes, Docker, and EC2.

I designed and configured monitoring components to collect infrastructure metrics, application metrics, container status, logs, and resource usage data. The monitoring system helped developers and operators understand whether the platform was running correctly, identify failures more quickly, and compare operational behavior across different deployment environments.

## Tech Stack

| Stack                           | Summary                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **AWS EKS**                     | Supported cloud-native deployment and monitoring for XCAP-Cloud on managed Kubernetes infrastructure.                |
| **On-premises Kubernetes(RKE2)** | Built monitoring support for Kubernetes clusters running in customer-controlled or internal on-premises environments. |
| **Docker / EC2**                | Supported containerized and VM-based deployment cases outside Kubernetes environments.                               |
| **Prometheus**                  | Collected infrastructure, container, and application metrics across different deployment environments.               |
| **Grafana**                     | Built dashboards to visualize system health, resource usage, application status, and operational metrics.            |
| **Loki**                        | Collected and queried application and system logs for troubleshooting.                                               |
| **Helm**                        | Managed Kubernetes monitoring components through reusable and configurable chart values.                             |
| **ArgoCD**                      | Supported GitOps-based deployment and synchronization of monitoring components.                                      |
| **Kubecost**                    | Helped monitor Kubernetes resource usage and cloud cost visibility for EKS-based environments.                       |


## Development & Maintenance Highlights
* Automated **Grafana initial setup**, including user creation, dashboard provisioning, and repeated configuration work, **removing the need for developer standby during late-night installations**.
* Reduced Helm chart configuration YAML from approximately **200 lines to 65 lines** by simplifying values and removing unnecessary settings.
* Compared **3 monitoring stack options** — ELK/EFK, PLG, and AWS CloudWatch — across **8 criteria** and selected PLG as the main monitoring direction.
* Built a **Docker-compose PLG prototype** and validated **4 core workflows**: metric collection, log collection, dashboard access, and troubleshooting.
* Expanded PLG monitoring across **AWS EKS, EC2, on-premises RKE2, and 4 internal servers** while keeping AWS costs predictable.
* Validated Docker-based monitoring through **12 load/performance test runs** on **4 on-premises 256GB RAM servers**.
* **Replaced manual log inspection** with **Grafana/Loki-based log search, filtering, and dashboard workflows** for System Engineering(25 total colleagues).
* Created **6 A-to-Z monitoring manuals**, documented **4 troubleshooting cases**, and delivered **6 hands-on / architecture guide sessions**.

| Deployment Environment | Kubernetes-Based Monitoring | Docker Compose-Based Monitoring |
| --- | --- | --- |
| **Cloud** | **AWS EKS**<br>staging server | **AWS EC2**<br>servers from global providers |
| **On-premises** | **RKE2**<br>On-premises Kubernetes environment | **Internal servers**<br>internal test servers |

## Actions
### Q1 2024 — Compared 3 Monitoring Stacks and Delivered 3 Technical Presentations

* Compared **3 monitoring stack options** — ELK/EFK, PLG, and AWS CloudWatch — and delivered **3 technical presentations** to support Cloud TF stack selection.
* Evaluated each option across **8 criteria**: metrics, logs, dashboards, alerts, scalability, operational complexity, documentation quality, and cost.
* Recommended **PLG** as the main monitoring direction after identifying **25–70% potential cost savings** compared with EFK, along with cloud-native architecture, Helm-based setup, horizontal scalability, and unified metric/log monitoring.
    * Researched AWS CloudWatch as a managed alternative, covering **7 AWS services/features** — Container Insights, Logs, SNS, Lambda, EventBridge, dashboards, and alerts — with an estimated monthly cost of approximately **$150**.
<p align="center">
   <img width="1320" height="419" alt="image" src="https://github.com/user-attachments/assets/02cc470f-5a10-4f23-b809-c56af0715b2a" />
</p>
<p align="center">
  <b>Left:</b> EFK vs. PLG comparison — selected PLG for 25–70% potential cost savings, unified metric/log monitoring and cloud-native scalability.<br>
  <b>Right:</b> AWS CloudWatch review — evaluated managed AWS monitoring flow using EKS, CloudWatch, SNS, Lambda, and alert delivery.
</p>

### Q2 2024 — Built 1 PLG Prototype, Validated 4 Workflows, Delivered 2 Hands-On Sessions
* Built the first working **Docker-compose PLG monitoring prototype** and deployed it to **2 internal test servers** for validation.
* Reduced manual troubleshooting work for the System Engineering team(25 total colleagues) by **replacing direct server log inspection** **with Grafana/Loki-based log search, filtering, and dashboard workflows**.
  * Proved the prototype across **4 core workflows**: metric collection, log collection, dashboard access, and troubleshooting.
* Delivered **2 hands-on usage guide sessions** for Cloud TF and System Engineering(25 total colleagues), helping other teams test the prototype and learn Grafana/Loki-based monitoring workflows.
    * Collected **2 weeks of feedback from the System Engineering Team(25 total colleagues)** and improved dashboard usability, documentation, and troubleshooting guidance.

<p align="center">
   <img width="700" alt="image" src="https://github.com/user-attachments/assets/a9f11d0b-d0b4-4062-b4f6-0046152f7fdb" />
</p>
<p align="center">
  <b>Docker-based PLG prototype architecture:</b> Prometheus for metrics, Loki for logs, and Grafana for visualization.
</p>

### Q3 2024 — Expanded PLG Monitoring Across 4 Environment Types and Validated 12 Test Runs Without Unexpected AWS Cost Issues

* **Deployed and stabilized** PLG monitoring across **AWS EKS, EC2, on-premises RKE2, and 4 internal servers** without unexpected AWS cost issues.
* **Validated Docker-based monitoring** through **12 load/performance test runs** on **4 on-premises 256GB RAM servers**, including **two-day weekend testing sessions**.
* Applied **5 feedback-based usability improvements** from the Q2 prototype review.
* Created **2 practical usage manuals** and delivered **2 architecture guide sessions** covering Docker-based and Kubernetes-based monitoring models.
* Standardized Helm chart versions and environment-specific settings to improve deployment consistency and reduce installation issues.

<img width="1046" height="492" alt="image" src="https://github.com/user-attachments/assets/d921c63d-bf7b-463d-8217-5abea21555e9" />
<p align="center">
  <b>Before:</b> Default Grafana home screen made it unclear which dashboard to open or what cluster status to check first.<br>
  <b>After:</b> Customized main dashboard shows key metrics immediately, including CPU/RAM usage, pod status, scheduling failures, container crashes, and system errors.
</p>


### Q4 2024 — Automated Grafana Setup, Removed 1 Developer Standby, and Reduced AWS Costs by 33%
* Automated Grafana initial setup, eliminating **1 developer standby requirement** during late-night installations and saving approximately **2 hours per setup** through automated user creation, dashboard provisioning, and configuration.
* Reduced AWS costs by **33%**, from approximately **$990 to $660 per month**, by installing and operating **Kubecost** for Kubernetes cost visibility.
* Delivered **2 additional hands-on sessions** to help engineers use Grafana dashboards, investigate logs, and follow monitoring workflows.
* Reduced Helm chart configuration YAML from approximately **200 lines to 65 lines** by simplifying values and removing unnecessary settings.
* Created **6 A-to-Z monitoring manuals** and documented **4 troubleshooting cases** for future maintenance.
* Migrated and upgraded Kubernetes monitoring Helm charts to improve availability, stability, scalability, and multi-cluster readiness.

<img width="1007" height="497" alt="image" src="https://github.com/user-attachments/assets/665e5559-7ab0-4902-9094-c6db36a04e23" />
<p align="center"><b>[Dashboards] Completed dashboard for Kubernetes monitoring </b></p>

<img width="1286" height="578" alt="image" src="https://github.com/user-attachments/assets/c4eaf977-3d7f-4a12-8496-302aa29aef1f" />
<p align="center"><b>[Guide Documents] A-to-Z monitoring guides and troubleshooting documents created for long-term maintenance.</b></p>



## Results

| Metric                                                               | Impact                                                                                                                                                                                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **33% AWS cost reduction**                                           | Used Kubecost to identify Kubernetes resource usage and cost optimization opportunities, helping reduce unnecessary AWS spending for the XCAP-Cloud EKS environment.                                                     |
| **$1.8M CAD projects reviewed Monitoring system for operational use** | Built an observability system that was reviewed as the monitoring foundation for projects worth approximately CAD 1.8M, covering performance monitoring, log monitoring, cost visibility, and troubleshooting workflows. |
| **5 internal seminars including demos and hands-on session**         | Helped System Engineers, Cloud Task Force, and other teams understand how to use the monitoring stack for troubleshooting and operation.                                                                                 |
| **6 A-to-Z technical guides**                                        | Reduced onboarding friction by documenting monitoring setup, dashboard usage, log investigation, and operational workflows.                                                                                              |

## Engineering Skills Improved

- Learned how to design observability for real production systems across different infrastructure environments.
    - Built monitoring support for AWS EKS, on-premises Kubernetes, Docker, and EC2 deployment cases.
    - Understood how infrastructure differences affect monitoring design, deployment strategy, and troubleshooting workflows.
    - Learned to think beyond application development and consider system health, operational visibility, and maintainability.
        
- Strengthened cloud-native and DevOps engineering skills through a company-wide SaaS transition project.
    - Worked with Kubernetes, Helm, ArgoCD, Prometheus, Grafana, Loki, and AWS EKS.
    - Designed reusable monitoring configurations that could be adapted to multiple environments.
    - Learned the importance of standardizing observability when moving from customized on-premises projects to scalable cloud-based delivery.

<p align="center"> <a href="https://github.com/Magpie1000/"> <img src="https://img.shields.io/badge/←%20Back%20to%20Main-24292f?style=for-the-badge" alt="Back to Main" /> </a> </p>
