# Describe Azure Compute and Networking Services

## Azure Virtual Machines

With Azure Virtual Machines (VMs), a user can create and use VMs within the cloud. Virtual Machines provide Infrastructure as a Service (IaaS) in the form of a virtualized server and can be used in various ways.

Virtual Machines are just like physical computers, allowing users to customize all of the software running on the VM. 

**VMs allow for:**
- Total control over the operating system.
- Ability to run custom software.
- Use of custom host configurations.

Azure VMs offer the flexibility of virtualization without having to buy or maintain the physical hardware that runs the VM itself. However, as an IaaS offering, you still need to configure, update, and maintain the software that runs on the VM.

Users can also use a pre-created **VM Image**. An image is a template used to create a VM and may already include an OS and other software such as development tools and web hosting environments.

## Scaling VMs in Azure

You can run single VMs for testing, development, or minor tasks. You can also group VMs together to provide high availability, scalability, and redundancy. Azure manages the grouping of VMs for you with features such as Scale Sets and Availability Sets.

### Virtual Machine Scale Sets
Scale Sets allow users to create and manage a group of identical, load-balanced VMs. With Scale Sets, Azure automates most of the work, allowing you to centrally manage, configure, and update a large number of VMs in minutes. 

- **Auto-scaling:** The number of VM instances can automatically increase or decrease in response to demand, or you can set it to scale based on a defined schedule. 
- **Efficiency:** Scale Sets automatically deploy a load balancer to ensure resources are being used efficiently. 
- **Use Case:** Building large-scale services for compute, big data, and container workloads.

### Virtual Machine Availability Sets
Availability Sets are another tool to assist in building a more resilient and highly available environment. They ensure that VMs stagger updates and have redundant power and network connectivity, preventing the potential loss of all VMs due to a single network or power failure.

**Availability Sets Accomplish:**
- **Update Domain (UD):** The update domain groups VMs that can be rebooted at the same time. This allows the user to apply updates while knowing that only one update domain grouping is offline at a time. An update group going through the update process is given a 30-minute recovery window before maintenance on the next update domain continues.
- **Fault Domain (FD):** The fault domain groups VMs by a common power source and network switch. By default, an availability set splits your VMs across up to three fault domains. This protects against a physical power or networking failure.

## When to Use Virtual Machines
- **Testing and Development:** Quickly creating and disposing of environments.
- **Running Applications in the Cloud:** Hosting apps that require specific OS configurations.
- **Extending Your Datacenter:** Connecting on-premises servers to the cloud.
- **Disaster Recovery:** Creating backup instances in case of a primary site failure.

## Move to the Cloud with VMs (Lift and Shift)
VMs are an excellent choice when moving from a physical server to the cloud. You can create an image of the physical server and host it within a VM with little to no change. Just like a physical on-premises server, you must maintain the virtual machine because you are responsible for maintaining the installed OS and software.

## Virtual Machine Resources
When you provision a VM, you will pick the resources associated with that instance:
- **Size:** (Determines CPU and RAM).
- **Storage Disks:** (Managed disks for data).
- **Networking:** (Virtual Network and IP configurations).
