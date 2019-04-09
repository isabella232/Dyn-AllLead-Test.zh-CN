---
title: Design Details - The Role of the Reorder Point
description: This topic highlights the importance of setting a reorder point, so that you when to order more inventory.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 4c1f49ef41e93eb777e192a38550cccc290b0fcd
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7296"
---
# <a name="design-details-the-role-of-the-reorder-point"></a>Design Details: The Role of the Reorder Point
In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.  
  
A reorder point represents demand during lead time. When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity. Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.  
  
Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.  
  
The reorder point reflects a certain inventory level. However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.  
  
## <a name="see-also"></a>See Also  
[Design Details: Reordering Policies](design-details-reordering-policies.md)   
[Design Details: Planning Parameters](design-details-planning-parameters.md)   
[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)