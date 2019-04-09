---
title: Design Details - Handling Reordering Policies
description: Overview of tasks for defining a reorder policy in supply planning.
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
ms.openlocfilehash: b2efe565a1cb19beb02b9674abfa7bff886d2ab4
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7316"
---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="b3348-103">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="b3348-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="b3348-104">For an item to participate in supply planning, a reorder policy must be defined.</span><span class="sxs-lookup"><span data-stu-id="b3348-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="b3348-105">The following four reordering policies exist:</span><span class="sxs-lookup"><span data-stu-id="b3348-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="b3348-106">Fixed Reorder Qty.</span><span class="sxs-lookup"><span data-stu-id="b3348-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="b3348-107">Maximum Qty.</span><span class="sxs-lookup"><span data-stu-id="b3348-107">Maximum Qty.</span></span>  
* <span data-ttu-id="b3348-108">Order</span><span class="sxs-lookup"><span data-stu-id="b3348-108">Order</span></span>  
* <span data-ttu-id="b3348-109">Lot-for-Lot</span><span class="sxs-lookup"><span data-stu-id="b3348-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="b3348-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span><span class="sxs-lookup"><span data-stu-id="b3348-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="b3348-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span><span class="sxs-lookup"><span data-stu-id="b3348-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="b3348-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span><span class="sxs-lookup"><span data-stu-id="b3348-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="b3348-113">In This Section</span><span class="sxs-lookup"><span data-stu-id="b3348-113">In This Section</span></span>  
[<span data-ttu-id="b3348-114">Design Details: The Role of the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="b3348-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="b3348-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="b3348-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="b3348-116">Design Details: The Role of the Time Bucket</span><span class="sxs-lookup"><span data-stu-id="b3348-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="b3348-117">Design Details: Staying under the Overflow Level</span><span class="sxs-lookup"><span data-stu-id="b3348-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="b3348-118">Design Details: Handling Projected Negative Inventory</span><span class="sxs-lookup"><span data-stu-id="b3348-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="b3348-119">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="b3348-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="b3348-120">See Also</span><span class="sxs-lookup"><span data-stu-id="b3348-120">See Also</span></span>  
[<span data-ttu-id="b3348-121">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="b3348-121">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)   
[<span data-ttu-id="b3348-122">Design Details: Planning Assignment Table</span><span class="sxs-lookup"><span data-stu-id="b3348-122">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)   
[<span data-ttu-id="b3348-123">Design Details: Central Concepts of the Planning System</span><span class="sxs-lookup"><span data-stu-id="b3348-123">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)   
[<span data-ttu-id="b3348-124">Design Details: Balancing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="b3348-124">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)   
[<span data-ttu-id="b3348-125">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="b3348-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)