# Azure Management and Governance

## Factors That Can Affect Costs in Azure

Azure shifts development costs from the capital expense (CapEx) of building out and maintaining infrastructure and facilities to an operational expense (OpEx) of renting infrastructure as you need, whether it's compute, storage, network, or any other needs.

**OpEx cost can be impacted by many factors:**
- Resource Type
- Consumption
- Maintenance
- Geography
- Subscription Type
- Azure Marketplace

## Resource Type

Multiple factors influence the cost of Azure resources. The type of resource, the settings of the resource, and the Azure region will have an impact on how much a resource costs. When provisioning an Azure resource, Azure creates metered instances for that resource; it will track that resource's usage and generate a usage record that can be used to **calculate** the bill.

## Consumption

Pay-as-you-go has been a consistent theme throughout. This is a cloud payment model that allows you to pay for the resources that you utilize during a billing cycle. If you use more compute in one cycle, you pay more; if you use less in the next cycle, you pay less. 

However, Azure offers the ability to commit to using a set amount of cloud resources in advance and **receiving** discounts on those reserved resources. Services such as databases, compute, and storage all provide the option to commit to a level of usage and receive a discount which can accumulate to about 72% of savings in some cases.

When you reserve capacity, you're committing to using and paying for a certain amount of Azure resources during a given period (1-3 years). The pay-as-you-go method allows you to go beyond your reserve capacity if needed and allows you to pay for the additional resources you exceeded past your reservation. This model allows for significant savings on reliable, consistent workloads while also having the flexibility to rapidly increase your cloud footprint as needs rise.

## Maintenance

The flexibility of the cloud makes it possible to adjust resources based on the level of demand. Using resource groups can help keep all of your resources organized. In order to control costs, it is **important** to maintain your cloud environment by **keeping an eye** on your resources and ensuring you're not keeping around resources that are no longer in use or needed, which can help in lowering your cloud costs.

## Geography

When provisioning a resource in Azure, you need to define a region where the resource deploys. Azure infrastructure is distributed globally and enables you to deploy your services centrally, closest to your customers, or something in between both.

Global deployment comes with global pricing differences. The cost of power, labor, taxes, and fees vary depending on the location; due to these variations, Azure resources can differ in price to deploy depending on the region.

Network traffic is also impacted based on the geography. It is generally less expensive to move information within Europe than to move information from Europe to Asia or South America.

## Network Traffic

Billing zones play a factor in determining the cost of some Azure services. A zone is a geographical grouping of Azure regions for billing purposes.

Bandwidth refers to data moving in and out of Azure datacenters.
- **Inbound data transfers:** Free (Data going into Azure datacenters).
- **Outbound data transfers:** Priced based on zones (Data leaving Azure datacenters).

## Subscription Type

Some Azure subscription types include usage allowances, which can affect potential costs.

## Azure Marketplace

Azure Marketplace allows you to purchase Azure-based solutions and services from third-party vendors. When you purchase products on the marketplace, you may pay not only for the Azure services you're using, but also for the services and expertise of the third-party vendor. 

**All solutions available in Azure Marketplace are certified and compliant with Azure policies and standards.**

## Pricing Calculator

The pricing caculator is designed to give an estimated for provisioning resources in Azure. You can get a estimate for individual resources, build out a solution, and use an example scenario to see an estimate of the Azure expense. This calculator allows to get a insight o fthe cost of provisioned resources in Azure.

You can estimate the cost of any provisioned resources, including compute, storage, and associated network costs. You can account for different storage option such as:
- Storage Types.
- Access Tier.
- Redundancy.

## Microsoft cost Management Tool

Cost management provides the ability to quickly assess Azure resource costs, create alerts based on resource spend, and create budgets that can be utilized to automate management of resources.

Cost analysis is a subnet of Cost management that provides a quick visual of your Azure costs. Using cost analysis, you can view the total cost in a variety of different ways, including by billing cycle, region, and resources.

You can use cost analysis to both explore and analyze your organizational costs. Visualize where costs are accrued and identify spending trends. Also allows to view accumulated costs over time to estimate monthly, quaterly, and yearly cost trends.

## Cost Alerts

Cost alerts provide a single location to check on all different alert types that may show up in the Cost management service. 

Three types of alerts:
- Budget Alerts.
- Credit Alerts.
- Department Spending Quota Alerts.

## Budget Alerts

Budget alerts notify you when spending, based on usage or cost, reaches or exceeds the amount defined in the alert condition of the budget. Cost management budgets are created using the Azure portal or the Azure comsumption API.

Within the Azure portal, budgets are defined by costs. Budgets are defined by cost or by the cost of consumption usage when using the Azure consumption API. Budget alert systems support both cost-based and usage-based budgets. Budget alerts are generated automatically whenever the budget alert condtions are met.

## Credit Alerts

Credit alerts notify when your Azure credit monetary commitments are consumed. Monetary commitments are for organizations with Enterprise Agreements (EAs). Credit alerts are generated automatically at 90% and 100% of your Azure credit balance.

## Department Spending Quota Alerts

Department spending quota alerts notify you when department spending reaches a fixed threshold of the quota. Spending qoutas are configured in the EA portal. Whenever a threshold is met, it generates a email to the department owners, and apears in the cost alerts.

