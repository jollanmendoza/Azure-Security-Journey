# Azure Management and Governance

Azure shifts development costs from the capital expense (CapEx) of building out and maintaining infrastructure and facilities to an operational expense (OpEx) of renting infrastructure as you need, whether it's compute, storage, network, or any other needs.

**OpEx cost can be impacted by many factors:**
- Resource Type
- Consumption
- Maintenance
- Geography
- Subscription Type
- Azure Marketplace

## Resource Type

Multiple factors influence the cost of Azure resources. The type of resource, the settings of the resource, and the Azure region will have a impact on how much a resource costs. When provisioning an Azure resource, Azure creates a metered instances for that resource and it will track that resources' usage and generate a usage record that can be used to caculate the bill.

## Consumption

Pay-as-you-go has been a consistent theme throughout, and that's how cloud payment model where allows you to pay for the resources that you utilize during a billing cycle. If you use more compute in one cycle, you pay more but if you less in the next cycle, you pay less. 

However, Azure offers the ability to commit to using a set amount of cloud resources in advance and recieving discounts on those reserved resources. Services such as databases, compute, and storage all provide the option to commit to a level of usage and recieve a discount which can accumulate to about 72% of savings in some cases.

When you reserve capacity, you're committing to using and paying for a certain amount of Azure resources during a given period (1-3 years). The pay-as-you-go method allows you to go beyond your reserve capacity if needed and allow you to pay for the additional resources you exceeded past your reservation. This model allows for significant savings on reliable, consistent workloads while also having the flexibility to rapidly increase your cloud footprint as needs rise.

## Maintenance

The flexibility of the cloud makes it possible to adjust resources based on the level of demand. Using resource groups can help keep all of your resources organized. In order to control costs, it is inportant to maintain your cloud environment by keeping a eye on your resources and ensuring you're not keeping around resources that are no longer in use or needed, which can help in lowering your cloud costs.

## Geography

When provisioning a resource in Azure, you need to define a region where the resource deploys. Azure infrastructure is distributed globally, and enables you to deploy your services centrally or closest to your customers, or something inbetween both.

Global deployment comes with global pricing differences. Cost of power, labor, taxes, and fees vary depending on the location, and due to these variations, Azure resources can differ in price to deploy depending on the region.

Network traffic also impacted based on the geography. It would less expensive to move information within Europe than to move information from Europe to Asia/South America.

## Network Traffic

Billing zones play a factor in determining the cost of some Azure services.

A zone is a geographical grouping of Azure regions for billing purposes.

Bandwidth refers to data moving in and out of Azure databases.
- Inbound data transfers are free. (Data going into Azure databases).
- Outbound data transfers are priced based on zones. (Data leaving Azure databases).

## Subscription Type

Some Azure subscription types include usage allowances, which can affect potential costs.

## Azure Marketplace

Azure Marketplace allows you to purchase Azure-Based solutions and services from third-party vendors. When you purchase products on the marketplace, you may not pay for not only the Azure services you're using, but also the services and expertise of the third-party vendor. 

**All solutions available in Azure Marketplace are certified and compliant with Azure policies and standards.**
