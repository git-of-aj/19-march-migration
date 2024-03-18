# MS Module - https://docs.microsoft.com/en-us/learn/modules/manage-hybrid-workloads-azure-arc/2-describe

# Azure Arc
Azure Arc expands the support for Azure Resource Manager to resources running outside of Azure. This means that a physical server or a VM running in an on-premises datacenter can be registered with Azure Resource Manager and presented as a compute resource to the fabric controller. This applies to any server running the Windows Server or Linux server in an on-premises datacenter or hosted by a third-party cloud provider.

> Azure Service Fabric is a distributed systems platform that makes it easy to package, deploy, and manage scalable and reliable microservices and containers
> You can create clusters for Service Fabric in many environments, including Azure or on premises, on Windows Server or Linux. You can even create clusters on other public clouds.
> Service Fabric powers many Microsoft services today, including Azure SQL Database, Azure Cosmos DB, Cortana, Microsoft Power BI, Microsoft Intune, Azure Event Hubs, Azure IoT Hub, Dynamics 365, Skype for Business, and many core Azure services.
> [source - MS Docs](https://learn.microsoft.com/en-us/azure/service-fabric/service-fabric-overview)

# Steps 
0. [Check if supported OS](https://learn.microsoft.com/en-us/azure/azure-arc/servers/prerequisites#supported-operating-systems)
1. Download -  Azure Connected Machine agent for SMALL SCALE - generate and run script in Azuer portal
- CAN ONBOARD Linux machines hosted on-premises or with another cloud provider
- Requires Permission - 
Azure Connected Machine OnboardingOnboard machines ==> Onboard machines

* Azure Connected Machine Resource Administrator ==> Read, modify, and delete a machine
**In larger environments, you can use the remote PowerShell scripting or a service principal l to perform the installation and registration in an unattended manner. Alternatively, you can automate the deployment using Configuration Manager or Group Policy.**
2. that resource has a unique Resource ID property. It belongs to a resource group inside a subscription, and it can benefit from Azure Resource Manager-based mechanisms such as Azure Policy and tags.
3. After you install the agent, it requires outbound connectivity to Azure Arc over Transmission Control Protocol (TCP) port 443

