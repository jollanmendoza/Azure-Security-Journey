# Azure Architecture

## What is Azure and What does it Provide?
Azure is a expanding set of cloud services that help meet current/future buisness challenges. Azure provides the user the freedom to build, manage, and deploy applications on a massive global network using well known tools and frameworks.

- **Azure Provides Limitless Innovation:** Allows users to build intelligent apps and solutions with advanced technology, tools, and services to elevate your buisness.
- **Brings Ideas to Life:** Develop on a trusted platform to advance your organization with industry-leading AI and cloud services.
- **Seamlessly Unify:** Efficently manage all your infrastructure, data, analytics, and AI solutions across an integrated platform.
- **Innovate On Trust:** Rely on trusted technology from a partner who's dedicated to security and responsibility.

## Interaction With Azure
**Azure Portal:** provides a graphic user interface (GUI) to interact with Azure services which include:
- Different service areas.
- Manage subscriptions & accounts.
- Search for specific services/settings.

Azure Portal allows for the usage of command line interface (CLI) with Powershell and BASH commands. The user also can switch between using either Powershell or BASH commands in a click of a button. When in Powershell mode, the command line starts with PS (PowerShell), and when in BASH mode, the command line starts with your username@azure.

**Most Azure specific commands begin with the letters az. (For both Powershell & BASH).**

**Azure CLI Interactive Mode:** This changes behavior to more resemble an integrated development enviroment. This mode provides autocompletion, command descriptions, and examples which is perfect for beginners who aren't used to using Powershell or BASH but want to still use the command line. (az interactive is the command to enter this mode).

## Azure Physical Infrastructure
The physical infrastructure for Azure starts with Datacenters.
 
  - Facilities with resources arranged in racks, dedicated power, cooling, and network infrastructure.

Microsoft Azure has these datacenters around the globe, but these individual datacenters aren't directly accessible. These datacenters are grouped into Azure Regions/Availability Zones that are designed to assist in achieving resiliency and reliability for buisness-critical workloads.

- **Azure Region:** A region is a geographical area on the planet that contains atleast one or more potential datacenters that are nearby and networked together with a low-laency network.

 - Azure assign and control the resources within each region to ensure workload are balanced, and as a user when deploying a resource within Azure, you'll often need to choose the region in which you need this resource to be deployed.

  - **Azure Availability Zones:** Physically separate datacenters within a Azure Region. Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking. An availability zone is setup to be an isolation boundary, and if one zone went offline, the other continues to work. Availability zones are connected through high-speed, private fiber-optic networks.
 - Can utilize availability zones to run mission-critical applications and build high availability into your application architecture by co-locating your compute, storage, networking, and data resources within an availability zone and replicating in other availability zones.
 - Availabiliy zones are primarily for virtual machines, managed disks, load balancers, and SQL databases.
Azure services that support availability zones fall into these three catagories:
- **Zone Services:** Pin the resource to a specific zone.
- **Zone-Redundant Services:** Teh platform replicates automatically across zones.
- **Non-Regional Services:** Services are always available from Azure geographies and are highly resilient to zone-wide outageas as well as region-wide outages.

