---
title: Setting Filters for Dynamic Allocation Bases
description: The dynamic allocation method is based on changeable values. For example, the number of employees in a cost center or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: e26f0a53fa9ded085e10bce3a6f0cda238db80d9
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "6948"
---
# <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases
The dynamic allocation method is based on changeable values. For example, the number of employees in a cost center or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.  

## <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases  
 The following table shows which filters are possible for different allocation bases and which values are valid in the **No. Filter** and **Group Filter** fields. Press F1 in the **Date Filter Code** field to read detailed descriptions.  

|**Base**|**No. Filter**|**Date Filter Code**|**Cost Center Filter**|**Cost Object Filter**|**Group Filter**|  
|--------------|----------------------------------------|----------------------------------------------|------------------------------------------------|------------------------------------------------|------------------------------------------|  
|G/L Entries|G/L Account|Yes|Yes|Yes|N/A|  
|G/L Budget Entries|G/L Account|Yes|Yes|Yes|G/L Budget Name|  
|Cost Type Entries|Cost Type|Yes|Yes|Yes|N/A|  
|Cost Budget Entries|Cost Type|Yes|Yes|Yes|Budget Name|  
|No of Employees|N/A|Yes|Yes|Yes|N/A|  
|Items Sold (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Sold (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  

## <a name="see-also"></a>See Also  
 [Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
 [How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md)   
 [Defining and Allocating Costs](finance-define-and-allocate-costs.md)
