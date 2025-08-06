# 💠 Azure KQL Queries Collection
This repository contains a curated collection of Kusto Query Language (KQL) queries for Azure Resource Graph, Log Analytics, and other Azure monitoring services. These queries help audit, monitor, and analyze Azure Virtual Machines and other resources efficiently.

> ⚙️ Some queries are ready for production use, while others are examples or templates for customization and learning.

---

## 📁 Repository Structure

Generally organized as follows:
kql/
├── VirtualNetwork
├── VirtualMachine
├── AppService
├── Storage


## 🚀 How to Use

You can run these queries directly in the Azure Resource Graph Explorer or Log Analytics workspace.

Example: Query all Azure VMs 

Resources
| where type == "microsoft.compute/virtualmachines"
| project 
    name, 
    location, 
    subscriptionId,
    resourceGroupName,