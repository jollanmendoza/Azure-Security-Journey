# Shared Responsibility Model

## Definition
The Shared Responsibility Model is a framework that identifies which security tasks are handled by the cloud provider (Microsoft) and which tasks are handled by the consumer (You). 

## Cloud Services Models
**Infrastructure as a Service (IaaS):** Places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity.

**Software as a Service (SaaS):** Places most of the responsibility with the cloud provider. 

**Platform as a Service (PaaS):** Being the middle ground between IaaS and SaaS, this rests in the middle and evenly distributes responsibility between the cloud provider and the consumer.

## Shared Responsibility Table
This table informs who is responsible for what (Customer, Microsoft, or Shared), depending on the cloud service type.

| Responsibility | SaaS | PaaS | IaaS | On-Premises |
| :--- | :--- | :--- | :--- | :--- |
| Information and Data | Customer | Customer | Customer | Customer
| Devices (PCs & Mobile) | Customer | Customer | Customer | Customer
| Acounts & Identities |  Customer | Customer | Customer | Customer
| Identity and Directory Infrastructure | Shared | Shared | Customer | Customer |
| Applications | Microsoft | Shared | Customer | Customer |
| Network Controls | Microsoft | Shared | Customer | Customer |
| Operating System | Microsoft | Microsoft | Customer | Customer |
| Physical Hosts | Microsoft |  Microsoft | Microsoft | Customer |
| Physical Network | Microsoft | Microsoft | Microsoft | Customer |
| Physical Datacenter | Microsoft | Microsoft | Microsoft | Customer|

When using a cloud provider, you'll always be responsible for:
- The information and data stored within the cloud.
- Devices that are allowed to connect to your cloud (cellphones, computers, and etc.)
- The accounts and identities of the users, services, and devices within your organization.

The cloud provider is always responsible for:
- The physical datacenter.
- The physical network.
- The physical hosts.

Your service model will determine responsibility for things such as:
- Operating systems.
- Network Controls.
- Applications.
- identity and Infrastructure.

