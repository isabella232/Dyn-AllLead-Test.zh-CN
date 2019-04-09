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
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="e451b-103">Design Details: The Role of the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="e451b-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="e451b-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span><span class="sxs-lookup"><span data-stu-id="e451b-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  
  
<span data-ttu-id="e451b-105">A reorder point represents demand during lead time.</span><span class="sxs-lookup"><span data-stu-id="e451b-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="e451b-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span><span class="sxs-lookup"><span data-stu-id="e451b-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="e451b-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span><span class="sxs-lookup"><span data-stu-id="e451b-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  
  
<span data-ttu-id="e451b-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span><span class="sxs-lookup"><span data-stu-id="e451b-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  
  
<span data-ttu-id="e451b-109">The reorder point reflects a certain inventory level.</span><span class="sxs-lookup"><span data-stu-id="e451b-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="e451b-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span><span class="sxs-lookup"><span data-stu-id="e451b-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="e451b-111">See Also</span><span class="sxs-lookup"><span data-stu-id="e451b-111">See Also</span></span>  
[<span data-ttu-id="e451b-112">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="e451b-112">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)   
[<span data-ttu-id="e451b-113">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="e451b-113">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)   
[<span data-ttu-id="e451b-114">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="e451b-114">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)   
[<span data-ttu-id="e451b-115">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="e451b-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)