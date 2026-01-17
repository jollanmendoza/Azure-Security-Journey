# Azure Architecture

## What is Azure and What does it Provide?
Azure is an expanding set of cloud services that help meet current and future **business** challenges. Azure provides the user the freedom to build, manage, and deploy applications on a massive global network using well-known tools and frameworks.

- **Azure Provides Limitless Innovation:** Allows users to build intelligent apps and solutions with advanced technology, tools, and services to elevate your*business.
- **Brings Ideas to Life:** Develop on a trusted platform to advance your organization with industry-leading AI and cloud services.
- **Seamlessly Unify:** Efficiently manage all your infrastructure, data, analytics, and AI solutions across an integrated platform.
- **Innovate On Trust:** Rely on trusted technology from a partner who is dedicated to security and responsibility.

## Interaction With Azure
**Azure Portal:** Provides a graphical user interface (GUI) to interact with Azure services which include:
- Different service areas.
- Manage subscriptions & accounts.
- Search for specific services/settings.

The Azure Portal allows for the usage of a Command Line Interface (CLI) with PowerShell and BASH commands. The user can switch between using either PowerShell or BASH commands at the click of a button. When in PowerShell mode, the command line starts with **PS**, and when in BASH mode, the command line starts with **username@azure**.

**Most Azure-specific commands begin with the letters `az` (for both PowerShell & BASH).**

**Azure CLI Interactive Mode:** This changes behavior to more closely resemble an Integrated Development Environment (IDE). This mode provides autocompletion, command descriptions, and examples, which is perfect for beginners who aren't used to using PowerShell or BASH but still want to use the command line. (`az interactive` is the command to enter this mode).

## Azure Physical Infrastructure

The physical infrastructure for Azure starts with Datacenters.
- Facilities with resources arranged in racks, dedicated power, cooling, and network infrastructure.

Microsoft Azure has these datacenters around the globe, but these individual datacenters aren't directly accessible. These datacenters are grouped into Azure Regions and Availability Zones that are designed to assist in achieving resiliency and reliability for business-critical workloads.

### Azure Regions
A region is a geographical area on the planet that contains at least one or more potential datacenters that are nearby and networked together with a low-latency network.
- Azure assigns and controls the resources within each region to ensure workloads are balanced.
- When deploying a resource within Azure, you will often need to choose the region in which you need this resource to be deployed.

### Azure Availability Zones
Physically separate datacenters within an Azure Region. Each Availability Zone is made up of one or more datacenters equipped with independent power, cooling, and networking. An Availability Zone is set up to be an isolation boundary; if one zone goes offline, the others continue to work. Availability Zones are connected through high-speed, private fiber-optic networks.
- Utilize Availability Zones to run mission-critical applications and build high availability into your application architecture by co-locating your compute, storage, networking, and data resources within an Availability Zone and replicating in other Availability Zones.
- Availability zones are primarily for virtual machines, managed disks, load balancers, and SQL databases.

**Azure services that support Availability Zones fall into these three categories:**
- **Zonal Services:** Pin the resource to a specific zone.
- **Zone-Redundant Services:** The platform replicates automatically across zones.
- **Non-Regional Services:** Services are always available from Azure geographies and are highly resilient to zone-wide outages as well as region-wide outages.

### Azure Region Pairs
Most Azure regions are paired with another region within the same geography at least **300 miles** away. This allows for the replication of resources across a geography that assists in reducing the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region.

**Advantages of Region Pairs:**
- **Recovery Priority:** If an extensive Azure outage occurs, one region out of every pair is prioritized to ensure at least one is restored as quickly as possible for applications hosted in that region pair.
- **Sequential Updates:** Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outages.
- **Data Residency:** Data continues to reside within the same geography as its pair for tax and law enforcement jurisdiction purposes.

## Azure Management Infrastructure

The management infrastructure includes Azure resources, resource groups, subscriptions, and management groups.

- **Azure Resource:** The basic building block of Azure. This includes anything you create, provision, and deploy (e.g., Virtual Machines, Databases, and Cognitive Services).

### Resource Groups
Resource groups are logical groupings of these resources. 
- While a resource group can contain many resources, a single resource can only be within one resource group at a time. 
- When you move a resource to a new group, it is no longer associated with the former group. 
- **Inherited Actions:** Actions applied to a resource group apply to all resources within it. For example, if you delete a resource group, all resources contained within it are also deleted.

### Azure Subscriptions
In Azure, subscriptions are a unit of management, billing, and scale. They allow you to logically organize resource groups and facilitate granular cost management.

- **Billing Boundary:** This determines how an Azure account is billed. You can create multiple subscriptions for different billing requirements. Azure generates separate billing reports and invoices for each subscription.
- **Access Control Boundary:** Azure applies access management policies at the subscription level. You can create separate subscriptions to reflect different organizational structures or security requirements.

#### Reasons to Create Additional Subscriptions:
- **Environments:** Creating separate subscriptions for development, testing, and production to isolate data for compliance reasons.
- **Organizational Structure:** Reflecting different departments (e.g., Finance, IT, Marketing) to manage access and resources independently.
- **Billing:** Isolating costs for specific projects or clients for easier accounting.

### Azure Management Groups
Azure management groups provide a scope level above subscriptions. You can organize subscriptions into management groups and apply governance conditions that are inherited by all subscriptions within that group.

**Key Facts of Management Groups:**
- **Scale:** Supports up to 10,000 management groups in a single directory.
- **Depth:** A management group tree can support up to six levels of depth (excluding the root and subscription levels).
- **Hierarchy:** Each management group and subscription can support only one parent.
