# Cloud Fundamentals

## Core Definition
**Cloud Computing:** Delivery of computing services over the internet which include common IT infrastructure such as virtual machines, storage, databases, and networking. 

## Cloud Deployment Models
- **Private Cloud:** A cloud service used by a single entity.
- **Public Cloud:** A cloud built, controlled, and maintained by a third-party cloud service provider.
- **Hybrid Cloud:** A computing environment that uses both private and public clouds in an interconnected environment.
- **Multi-Cloud:** A scenario where an organization uses multiple public cloud providers (e.g., Azure and AWS). 

## Key Comparative Aspects Between Cloud Models
| Private Cloud | Public Cloud | Hybrid Cloud |
| :--- | :--- | :--- |
| Organizations have complete control over both resources and security. | No capital expenditures (CapEx) to scale up. | Provides the most flexibility for diverse workloads. |
| Data is not collocated with other organizations' data. | Applications can be quickly provisioned and deprovisioned. | Organizations determine exactly where to run their applications. |
| Hardware must be purchased for startup and maintenance. | Organizations pay only for what they utilize (OpEx). | Organizations maintain control over specific security or legal requirements. |
| Organizations are responsible for hardware maintenance and updates. | Organizations do not have complete control over underlying hardware. | Supports **"Cloud Bursting"** to handle heavy spikes of traffic using public resources. |

## Benefits of Cloud Computing

- **High Availability:** Ability to keep a system up and running for a long period (minimal downtime) even if components fail.
- **Scalability:** The ability to handle increases in demand.
    - **Vertical Scaling:** Increasing the "power" of an existing server (adding RAM/CPU).
    - **Horizontal Scaling:** Adding more servers (instances) to share the load.
- **Elasticity:** The ability to automatically scale resources (up or down) dynamically based on real-time demand.
- **Reliability:** The ability of a system to recover from failures and continue to function.
- **Predictability:**
    - **Performance:** Ensuring the speed and quality of the service remains consistent.
    - **Cost:** Being able to forecast and track cloud spend accurately.
- **Security & Governance:** Using built-in cloud tools to ensure the environment meets compliance standards.

## Cloud Economics
- **Consumption-Based Model:** Only pay for the resources you utilize.
- **CapEx (Capital Expenditure):** One-time, upfront expenditure to purchase or secure physical infrastructure.
- **OpEx (Operational Expenditure):** Ongoing spending on services or products over time.

# Describe Cloud Service Types.

## Infrastructure as a Service (IaaS)

Infrastructure as a Service (IaaS) is the most flexible category of cloud services due to it providing the maximum amount of control for your cloud resources. Within an IaaS model, the cloud provider is responsible for maintaining the hardware, network connectivity, and physical security. 

**Responsible for:**
- Operating System Installation.
- Configuration.
- Maintenance.
- Network Configuration.
- Database and Storage Configuration.

With IaaS, you're essentially renting the hardware in a cloud datacenter, but what you choose to do with that hardware is up to the user.

Within the shared responsibility model, IaaS places the largest share of responsibility with you. The cloud provider's responsibility is for maintaining the physical infrastructure and its access to the internet. You are responsible for installation and configuration, patching and updates, and most importantly, security.

## Platform as a Service (PaaS)

Platform as a Service (PaaS) is a middle ground between renting space in a datacenter (IaaS) and paying for a complete and deployed solution (SaaS). Within a PaaS environment, the cloud provider maintains the physical infrastructure, physical security, and connection to the internet. 

**Maintain:**
- Operating Systems.
- Middleware.
- Development Tools.
- Business Intelligence Services.

In PaaS, you don't have to stress about the licensing or patching for operating systems and databases. PaaS is well-suited to provide a complete development environment without the headache of maintaining all the development infrastructure.

Within the shared responsibility model, PaaS splits the responsibility between you and the cloud provider. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet just like IaaS. But in the PaaS model, the cloud provider will also maintain the operating systems, databases, and development tools.

Depending on the configuration, you and the cloud provider may be responsible for networking settings and connectivity within your cloud environment, network and application security, and the directory infrastructure.

## Software as a Service (SaaS)

Software as a Service (SaaS) is the most complete cloud service model from a product perspective. With SaaS, you're essentially renting or using a fully developed application. 

**SaaS Implementation:**
- Email.
- Financial Software.
- Messaging Applications.
- Connectivity Software.

The SaaS model is not known to be the most flexible, but it is easy to get up and running.

Within the shared responsibility model, SaaS is the model that places the most responsibility with the cloud provider and the least on the user. Within a SaaS environment, you're responsible for the data you put into the system, devices that are connected to the system, and the users who have access to it. Everything else falls onto the cloud provider; they're responsible for physical security of the datacenters, power, network connectivity, and the application development and patching.
