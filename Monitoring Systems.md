# SaaS Enablement & Monitoring System for XCAP-Cloud
## Project summary
<a href="https://www.ligaccuver.com/pages/eng/main.asp"> <img width="221" height="27" alt="LIG Accuver" src="https://github.com/user-attachments/assets/c31a1ad4-b9f9-4e4e-bb35-cb0c0703760c" /> </a> 

Served as a DevOps / Cloud Monitoring engineer in a LIG Accuver's company-wide task force to prepare XCAP-Cloud for SaaS and cloud-based deployment.

**The goal** of the task force was to make the **existing XCAP-Cloud platform deployable across multiple infrastructure environments**, including AWS EKS, on-premise Kubernetes, Docker-based deployments, and EC2. 

| Metric                         | Result                      | Impact                                                                                                         |
| ------------------------------ | --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **$1.1M / year**               | **Revenue**                 | served as sole full-stack developer for 3 projects of $1.1M CAD/year for 2 leading mobile carriers in Korea    |
| **2 + years**                  | **0 complaints**            | Handeled 3 projects for 2 years without any complaints.                                                        |
| **100% Client retention rate** | **2 Major mobile carieers** | Acieved 100% client retention rate with successfully developing and maintaining 3 projects with no complaints. |

## Background
### LIG Accuver
[LIG Accuver](https://www.ligaccuver.com/pages/eng/main.asp) is wireless network testing and analysis company that generated approximately CAD 186 million in revenue in 2025. It provides software solutions to major mobile carieers in Korea, North America and Europe, for measuring, analyzing, and visualizing mobile network performance. 

### XCAP-Cloud
**XCAP-Cloud** was the project platform I worked on at LIG Accuver. It is a web-based post-processing system that helps telecom engineers analyze wireless network measurement data, visualize test results, and troubleshoot network failures through charts, maps, tables, reports, and detailed log analysis.

<img width="3259" height="2475" alt="XCAP" src="https://github.com/user-attachments/assets/0a73b1cc-1837-4780-a415-a08e28014347" />

[Demo video of XCAP-Cloud](https://youtu.be/soPRkdRXi0g?si=9xyGWG3Y6Rg-kxIT)

## My Role / Responsibilities
My main responsibility was to build a monitoring system for XCAP-Cloud across four deployment environments: AWS EKS, on-premise Kubernetes, Docker, and EC2.

I designed and configured monitoring components to collect infrastructure metrics, application metrics, container status, logs, and resource usage data. The monitoring system helped developers and operators understand whether the platform was running correctly, identify failures more quickly, and compare operational behavior across different deployment environments.

## Tech stack

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


## Action
### Development Highlights 


More to come...

https://docs.google.com/presentation/d/1nV7nl2ik3LvQdGOb05OGBLeqbxMuGhPVFgi4tUe-0XY/edit?usp=sharing

https://docs.google.com/presentation/d/1qDeYAhviwo_KtIIOGKnNgqAm_ps_gTjju8yCiThxF9g/edit?usp=sharing

https://docs.google.com/presentation/d/1hXU2GqlQA9wcMu_3B68KOMODap8HBsRyI53MrW25J2I/edit?usp=sharing





### Maintenance and Optimization Highlights

More to come...

<img width="1468" height="676" alt="image" src="https://github.com/user-attachments/assets/b7afe9b7-3da9-4021-95ab-1ef294d82e23" />




## Result

| Metric                  | Result                                             | Impact                                                                                                                                                                                                                   |
| ----------------------- | -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **33%**                 | **AWS cost reduction**                             | Used Kubecost to identify Kubernetes resource usage and cost optimization opportunities, helping reduce unnecessary AWS spending for the XCAP-Cloud EKS environment.                                                     |
| **$1.8M CAD projects**  | **Monitoring system reviewed for operational use** | Built an observability system that was reviewed as the monitoring foundation for projects worth approximately CAD 1.8M, covering performance monitoring, log monitoring, cost visibility, and troubleshooting workflows. |
| **5 internal seminars** | **Technical sharing and demos**                    | Helped SE, Cloud TF, and other teams understand how to use the monitoring stack for troubleshooting and operation.                                                                                                       |
| **6**                   | **A-to-Z technical guides**                        | Reduced onboarding friction by documenting monitoring setup, dashboard usage, log investigation, and operational workflows.                                                                                              |

## Takeaways

- Learned how to design observability for real production systems across different infrastructure environments.
    - Built monitoring support for AWS EKS, on-premise Kubernetes, Docker, and EC2 deployment cases.
    - Understood how infrastructure differences affect monitoring design, deployment strategy, and troubleshooting workflows.
    - Learned to think beyond application development and consider system health, operational visibility, and maintainability.
        
- Strengthened cloud-native and DevOps engineering skills through a company-wide SaaS transition project.
    - Worked with Kubernetes, Helm, ArgoCD, Prometheus, Grafana, Loki, and AWS EKS.
    - Designed reusable monitoring configurations that could be adapted to multiple environments.
    - Learned the importance of standardizing observability when moving from customized on-premise projects to scalable cloud-based delivery.

