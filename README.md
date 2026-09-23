<div align="center">
  <img src="assets/banner.png" alt="Amin Azad — Azure Cloud, Platform Engineering and Security" width="100%" />
</div>

<p align="center">
  <strong>Azure Cloud Engineer · AZ-104 · M.Sc. Computer Science and Engineering, DTU</strong><br />
  Azure · AKS · Terraform · Kubernetes · Helm · GitHub Actions · Argo CD · Cloud Security
</p>

<p align="center">
  <a href="https://learn.microsoft.com/credentials/certifications/azure-administrator/"><img src="https://img.shields.io/badge/Microsoft_Certified-Azure_Administrator_Associate-0078D4?style=flat-square&amp;logo=microsoftazure&amp;logoColor=white" alt="Microsoft Certified Azure Administrator Associate" /></a>
  <a href="https://github.com/Amin-Azad"><img src="https://img.shields.io/badge/Focus-Azure_Cloud_%26_Platform_Engineering-0B1F33?style=flat-square" alt="Azure Cloud and Platform Engineering" /></a>
  <a href="https://www.linkedin.com/in/azadamin079/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn" /></a>
</p>

I am an Azure cloud and platform engineer based in Copenhagen. My portfolio is focused on practical Azure engineering: infrastructure, Kubernetes, identity, networking, CI/CD, GitOps, observability, security and recovery.

**Portfolio status:** CloudNest and the Azure 3-Tier CLI project are released as `v1.0.0`; the Nordic Shopping cloud-transformation case study is finalized; NordicShop AKS is my main platform-engineering project.

## About me

I am AZ-104 certified and hold a cybersecurity-focused M.Sc. in Computer Science and Engineering from the Technical University of Denmark (DTU).

I learn best by building systems, deploying them, breaking parts of them on purpose, and then verifying the recovery path. My projects include live Azure deployments, Terraform, Bicep, AKS, Helm, GitHub Actions, Argo CD, workload identity, private networking, tenant isolation, monitoring and controlled failure testing.

Before focusing on cloud engineering, I worked in IT support and digital transformation, including supporting more than 100 users across hardware, software and networking. That experience still shapes how I work: understand the problem, make the change, verify it, document the evidence and keep the system maintainable.

## Featured project

### [NordicShop — Azure AKS platform](https://github.com/Amin-Azad/nordicshop-aks-platform)

My main cloud/platform engineering project: a small multi-tenant marketplace used to build and operate an Azure Kubernetes platform end to end.

- reusable Terraform modules for Azure infrastructure
- AKS, VNet, ACR, Key Vault, managed identities, RBAC and remote Terraform state
- Kubernetes workloads packaged with Helm and reconciled by Argo CD
- GitHub Actions with Azure OIDC and immutable ACR image digests
- separate AKS Workload Identities for the API and database administration path
- per-secret Key Vault RBAC instead of shared vault-wide access
- PostgreSQL Row-Level Security plus API-level tenant authorization
- Azure Managed Prometheus, Managed Grafana and alerting
- controlled recovery tests for invalid images and PostgreSQL outages
- tenant-isolation verification: 11 passed / 0 failed
- PostgreSQL RLS lab: 18 passed / 0 failed
- final Terraform plan: no drift
- final Argo CD state: Synced / Healthy

The application is intentionally simple. The main goal is the platform around it: infrastructure, delivery, identity, security, observability and recovery.

## Other Azure projects

### [CloudNest — verified Azure infrastructure with Bicep](https://github.com/Amin-Azad/cloudnest-bicep)

A production-style Azure design with a smaller portfolio profile that I deployed successfully in Sweden Central, verified from the live environment and cleaned up afterward.

- modular Bicep with GitHub Actions and Azure OIDC
- App Service, Azure SQL, VNet integration, private endpoints and private DNS
- SQL, Storage and Key Vault with public network access disabled
- system-assigned Managed Identity with scoped Key Vault and Storage RBAC
- Log Analytics, Application Insights, diagnostics, alerts and Azure Policy
- guarded validation, What-If, deployment and cleanup workflows
- 32 live Azure resources verified before cleanup
- Azure Policy reported 31 / 31 evaluated resources compliant
- released as `v1.0.0`

The larger design includes Front Door, WAF, autoscale, a deployment slot and a secondary App Service region. I keep that separate from the smaller profile I actually deployed so the repository does not claim full regional data recovery.

### [Nordic Shopping — Azure cloud transformation case study](https://github.com/Amin-Azad/nordic-shopping-cloud-transformation)

An end-to-end infrastructure and deployment-automation case study for a fictional Copenhagen e-commerce business.

- multi-region Azure design using West Europe and Sweden Central
- modular subscription-scope Bicep with development and production parameters
- Front Door, WAF, App Service, Azure SQL, Key Vault and private networking
- GitHub Actions OIDC with validation, What-If, guarded deployment and cleanup
- cost estimation, security assessment, migration planning and recovery design
- controlled Azure deployment attempts with root-cause analysis, regression fixes and verified cleanup

This project is mainly about architecture, migration planning, deployment controls and learning from real subscription limits rather than presenting an unverified full production deployment.

### [Azure 3-Tier Infrastructure — Azure CLI and Bash](https://github.com/Amin-Azad/azure-3tier-cli-project)

A real Azure deployment built directly with Azure CLI and modular Bash scripts.

- four-subnet VNet with separate NSGs
- Standard Load Balancer and Linux web/application VMs
- Storage Account, Blob containers and Azure File Share
- Entra ID group, user-assigned Managed Identity and scoped RBAC
- Log Analytics, diagnostic settings and Recovery Services Vault
- live validation across networking, compute, storage, identity, monitoring and backup
- cleanup automation with deletion verification
- lightweight GitHub Actions repository validation
- deployment evidence retained with unnecessary Azure identifiers redacted
- released as `v1.0.0`

I keep this repository focused on direct Azure CLI and Bash automation rather than converting it into another Bicep or Terraform project.

## Technical focus

| Area | Tools and services |
| --- | --- |
| Azure | Azure Portal, Azure CLI, App Service, Azure SQL, Storage, ACR, Key Vault |
| Infrastructure as code | Terraform, Bicep, remote state, ARM deployment scopes, What-If |
| Containers and Kubernetes | Docker, Docker Compose, Kubernetes, AKS, Helm |
| CI/CD and GitOps | GitHub Actions, Azure OIDC, Argo CD, immutable image digests |
| Networking | VNets, subnets, NSGs, Load Balancer, private endpoints, private DNS, Front Door, WAF, Gateway API |
| Identity and security | Microsoft Entra ID, Managed Identity, Workload Identity, Azure RBAC, Key Vault, least privilege |
| Observability | Azure Monitor, Log Analytics, Managed Prometheus, Managed Grafana, alerts |
| Data and platform security | PostgreSQL, Row-Level Security, Redis, tenant isolation |
| Scripting and tools | Bash, PowerShell, Python, SQL, Git, GitHub, Linux, WSL2 |

## Cybersecurity and academic background

**M.Sc. in Computer Science and Engineering — Technical University of Denmark (DTU), 2023–2025**

Specialization: cybersecurity, networking, system security and distributed systems.

My master's thesis, *Blockchain-Enabled Cybersecurity for Cyber-Ship Systems: A Risk Assessment Approach*, examined maritime cybersecurity resilience, incident response and risk assessment using ISO 27001/27005.

Selected security work includes access-control implementation, incident-response runbooks, network attack analysis with Wireshark and Suricata, OWASP Juice Shop testing, and phishing detection using machine-learning models.

**B.Sc. in Computer Science and Engineering — North South University, 2015–2019**

## What I am looking for

I am interested in Azure cloud, platform, infrastructure, DevOps and cloud-security roles where I can work with real infrastructure, automation, operations and reliability.

I bring AZ-104 certification, a cybersecurity-focused DTU master's degree, previous IT support experience and practical Azure project work covering deployment, troubleshooting, security, monitoring and recovery.

I am primarily interested in opportunities in Denmark and am also open to relevant roles elsewhere in Europe.

## Contact

- [LinkedIn](https://www.linkedin.com/in/azadamin079/)
- [Email](mailto:azadamin079@gmail.com)
- Copenhagen, Denmark

<p align="center">
  <sub>Infrastructure claims on this profile are linked to code, workflow history or deployment evidence in the relevant repositories.</sub>
</p>
