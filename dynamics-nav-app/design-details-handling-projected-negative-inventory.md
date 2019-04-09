---
title: Design Details - Handling Projected Negative Inventory
description: The reorder point expresses the anticipated demand during the lead time of the item. When the reorder point is passed, it is time to order more. But the projected inventory must be large enough to cover the demand until the new order is received. Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.
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
ms.openlocfilehash: b4e127d8dd87ef963578efcfc92d7ad93b6ba075
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7048"
---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="a29f5-106">Design Details: Handling Projected Negative Inventory</span><span class="sxs-lookup"><span data-stu-id="a29f5-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="a29f5-107">The reorder point expresses the anticipated demand during the lead time of the item.</span><span class="sxs-lookup"><span data-stu-id="a29f5-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="a29f5-108">When the reorder point is passed, it is time to order more.</span><span class="sxs-lookup"><span data-stu-id="a29f5-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="a29f5-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span><span class="sxs-lookup"><span data-stu-id="a29f5-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="a29f5-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span><span class="sxs-lookup"><span data-stu-id="a29f5-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="a29f5-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span><span class="sxs-lookup"><span data-stu-id="a29f5-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="a29f5-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span><span class="sxs-lookup"><span data-stu-id="a29f5-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="a29f5-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span><span class="sxs-lookup"><span data-stu-id="a29f5-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="a29f5-114">Instead, it will reflect the exact deficiency.</span><span class="sxs-lookup"><span data-stu-id="a29f5-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="a29f5-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span><span class="sxs-lookup"><span data-stu-id="a29f5-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="a29f5-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span><span class="sxs-lookup"><span data-stu-id="a29f5-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 <span data-ttu-id="a29f5-117">![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")</span><span class="sxs-lookup"><span data-stu-id="a29f5-117">![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")</span></span>  

1.  <span data-ttu-id="a29f5-118">Supply **A**, initial projected inventory, is below reorder point.</span><span class="sxs-lookup"><span data-stu-id="a29f5-118">Supply **A**, initial projected inventory, is below reorder point.</span></span>  

2.  <span data-ttu-id="a29f5-119">A new forward-scheduled supply is created (**C**).</span><span class="sxs-lookup"><span data-stu-id="a29f5-119">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="a29f5-120">(Quantity = Maximum Inventory – Projected Inventory Level)</span><span class="sxs-lookup"><span data-stu-id="a29f5-120">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  

3.  <span data-ttu-id="a29f5-121">Supply **A** is closed by demand **B**, which is not fully covered.</span><span class="sxs-lookup"><span data-stu-id="a29f5-121">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="a29f5-122">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span><span class="sxs-lookup"><span data-stu-id="a29f5-122">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  

4.  <span data-ttu-id="a29f5-123">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span><span class="sxs-lookup"><span data-stu-id="a29f5-123">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  

5.  <span data-ttu-id="a29f5-124">Demand **B** is closed (creating a reminder to the projected inventory).</span><span class="sxs-lookup"><span data-stu-id="a29f5-124">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  

6.  <span data-ttu-id="a29f5-125">The new supply **D** is closed.</span><span class="sxs-lookup"><span data-stu-id="a29f5-125">The new supply **D** is closed.</span></span>  

7.  <span data-ttu-id="a29f5-126">Projected Inventory is checked; reorder point has not been crossed.</span><span class="sxs-lookup"><span data-stu-id="a29f5-126">Projected Inventory is checked; reorder point has not been crossed.</span></span>  

8.  <span data-ttu-id="a29f5-127">Supply **C** is closed (no more demand exists).</span><span class="sxs-lookup"><span data-stu-id="a29f5-127">Supply **C** is closed (no more demand exists).</span></span>  

9. <span data-ttu-id="a29f5-128">Final check: No outstanding inventory level reminders exist.</span><span class="sxs-lookup"><span data-stu-id="a29f5-128">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a29f5-129">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="a29f5-129">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="a29f5-130">This concludes the description of central principles relating to inventory planning based on reordering policies.</span><span class="sxs-lookup"><span data-stu-id="a29f5-130">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="a29f5-131">The following section describes the characteristics of the four supported reordering policies.</span><span class="sxs-lookup"><span data-stu-id="a29f5-131">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a29f5-132">See Also</span><span class="sxs-lookup"><span data-stu-id="a29f5-132">See Also</span></span>  
 [<span data-ttu-id="a29f5-133">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="a29f5-133">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)   
 [<span data-ttu-id="a29f5-134">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="a29f5-134">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)   
 [<span data-ttu-id="a29f5-135">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="a29f5-135">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)   
 [<span data-ttu-id="a29f5-136">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="a29f5-136">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
