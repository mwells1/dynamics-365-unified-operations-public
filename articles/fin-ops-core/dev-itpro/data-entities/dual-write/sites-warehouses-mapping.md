---
# required metadata

title: Integrated sites and warehouses
description: This topic describes the integration of site and warehouse data between Finance and Operations and Dataverse.
author: t-benebo
ms.date: 10/09/2019
ms.topic: article
ms.prod: 
ms.technology: 

# optional metadata

ms.search.form: 
# ROBOTS: 
audience: Application User, IT Pro
# ms.devlang: 
ms.reviewer: rhaertle
# ms.tgt_pltfrm: 
ms.custom: 
ms.assetid: 
ms.search.region: global
ms.search.industry: 
ms.author: benebotg
ms.dyn365.ops.version: 
ms.search.validFrom: 2019-08-15

---

# Integrated sites and warehouses

[!include [banner](../../includes/banner.md)]

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]



This topic describes the integration of site and warehouse data between Finance and Operations and Dataverse. Operational sites and warehouses are common concepts in a Supply Chain Management application. They are used to model the supply chain of your company.

## Templates

With the integration with Dataverse, these concepts and all their related information are available in Dataverse using the sites and warehouses data tables in the following table.

Finance and Operations apps | Other Dynamics 365 apps | Description
--------------------------|---------------------------|---
Sites | msdyn_operationalsites | 
Warehouses | msdyn_warehouses | 

[!include [symbols](../../includes/dual-write-symbols.md)]

[!include [operational sites](includes/InventOperationalSiteEntity-msdyn-operationalsite.md)]

[!include [warehouses](includes/InventWarehouseEntity-msdyn-warehouse.md)]



[!INCLUDE[footer-include](../../../../includes/footer-banner.md)]