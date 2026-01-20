# Describe Azure Compute and Networking Services

## Describe Azure Virtual Machines

With Azure Virtual Machines (VMs), a user can create and use VMs within the cloud. Virtual Machines provide IaaS in the form of a virtualized server and can be used in various ways.

Virtual Machines are just like phyiscal computers, allowing users to customize all of the software running on your VM. 

VMs can be used to:
- Control over the operating system.
- Ability to run custom software.
- Use custom host configurations.

Azure VMs offer flexibility of virtualization without having to either buy or maintain the physical hardware that runs the VM itself, but as an IaaS offering, you still need to configure, update, and maintain the software that runs on the VM.

Can also use a already created VM image. An image is a template used to create a VM and may already include an OS and other software such as development tools and web hosting environments.

# Scale VMs in Azure

Run single VMs for testing, development, or minor tasks. Also can group VMs together to provide high availability, scalability, and redundancy. Azure also manage the grouping of VMs for you with features such as Scale Sets and Availability Sets.

## Virtual Machine Scale Sets

## Virtual Machines availability Sets

Virtual machines availability sets another tool to assist in building a more resilient and highly avaiable environment. Availability sets are designed to ensure that VMs stagger updates and have multiple power and network connectivity, preventing potential lose of all your VMs with a single network or power failure.

Availability sets acommplish:
- **Update Domain:** The update domain group VMs that can be rebooted at the same time. This allows the user to apply updates while knowing that only one update domain grouping is offline at a time. All of the machines in a one upddate domain update. An update group going through the update process is given 30 min time to recover before maintenance on the next update domain continues.
- **Fault Domain:** The fault domain groups your VMs by common power source and network switch. By default, an availability set splits your VMs across up to three fault domains. This asissts in protecting against a physical power or networking failure by having VMs in different fault domains.

## When to Use Virtual Machines
- **During Testing and Development.**
- **When Running Applications In The Cloud.**
- **When Extending Your DataCenter.**
- **During Disaster Recovery.**
