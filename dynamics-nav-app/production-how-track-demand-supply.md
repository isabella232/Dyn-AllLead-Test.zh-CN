---
title: How to Track Relations Between Demand and Supply
description: From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/06/2017
ms.author: sgroespe
ms.openlocfilehash: c34ca81c94798daa7eebb75216299cf2233c2ca6
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7333"
---
# <a name="how-to-track-relations-between-demand-and-supply"></a><span data-ttu-id="dc595-103">How to: Track Relations Between Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="dc595-103">How to: Track Relations Between Demand and Supply</span></span>
<span data-ttu-id="dc595-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span><span class="sxs-lookup"><span data-stu-id="dc595-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span></span>

<span data-ttu-id="dc595-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span><span class="sxs-lookup"><span data-stu-id="dc595-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span></span> <span data-ttu-id="dc595-106">For more information, see the "Untracked Planning Elements" section.</span><span class="sxs-lookup"><span data-stu-id="dc595-106">For more information, see the "Untracked Planning Elements" section.</span></span>

## <a name="to-track-linked-items"></a><span data-ttu-id="dc595-107">To track linked items</span><span class="sxs-lookup"><span data-stu-id="dc595-107">To track linked items</span></span>
<span data-ttu-id="dc595-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span><span class="sxs-lookup"><span data-stu-id="dc595-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span></span>

<span data-ttu-id="dc595-109">The following describes how to track linked items on a firm planned production order.</span><span class="sxs-lookup"><span data-stu-id="dc595-109">The following describes how to track linked items on a firm planned production order.</span></span> <span data-ttu-id="dc595-110">The steps are similar for all other order types, and from planning worksheet lines.</span><span class="sxs-lookup"><span data-stu-id="dc595-110">The steps are similar for all other order types, and from planning worksheet lines.</span></span>

1. <span data-ttu-id="dc595-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="dc595-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="dc595-112">Open the relevant firm planned production order from the list.</span><span class="sxs-lookup"><span data-stu-id="dc595-112">Open the relevant firm planned production order from the list.</span></span>
3. <span data-ttu-id="dc595-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span><span class="sxs-lookup"><span data-stu-id="dc595-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span></span>

<span data-ttu-id="dc595-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span><span class="sxs-lookup"><span data-stu-id="dc595-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span></span>

## <a name="untracked-planning-elements"></a><span data-ttu-id="dc595-115">Untracked Planning Elements</span><span class="sxs-lookup"><span data-stu-id="dc595-115">Untracked Planning Elements</span></span>
<span data-ttu-id="dc595-116">The **Untracked Planning Elements** window opens when you choose the **Untracked Qty.** field in the **order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="dc595-116">The **Untracked Planning Elements** window opens when you choose the **Untracked Qty.** field in the **order Planning** window.</span></span> <span data-ttu-id="dc595-117">It serves two purposes:</span><span class="sxs-lookup"><span data-stu-id="dc595-117">It serves two purposes:</span></span>

1. <span data-ttu-id="dc595-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking window to see untracked quantities.</span><span class="sxs-lookup"><span data-stu-id="dc595-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking window to see untracked quantities.</span></span>
2. <span data-ttu-id="dc595-119">To hold warning messages displayed when the user chooses the **Warning** icon in the **Planning Worksheet** window.</span><span class="sxs-lookup"><span data-stu-id="dc595-119">To hold warning messages displayed when the user chooses the **Warning** icon in the **Planning Worksheet** window.</span></span>

<span data-ttu-id="dc595-120">The window contains entries which account for an untracked surplus quantity in order tracking network.</span><span class="sxs-lookup"><span data-stu-id="dc595-120">The window contains entries which account for an untracked surplus quantity in order tracking network.</span></span> <span data-ttu-id="dc595-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span><span class="sxs-lookup"><span data-stu-id="dc595-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span></span> <span data-ttu-id="dc595-122">This untracked surplus can come from:</span><span class="sxs-lookup"><span data-stu-id="dc595-122">This untracked surplus can come from:</span></span>

- <span data-ttu-id="dc595-123">Production forecast</span><span class="sxs-lookup"><span data-stu-id="dc595-123">Production forecast</span></span>
- <span data-ttu-id="dc595-124">Blanket orders</span><span class="sxs-lookup"><span data-stu-id="dc595-124">Blanket orders</span></span>
- <span data-ttu-id="dc595-125">Safety stock quantity</span><span class="sxs-lookup"><span data-stu-id="dc595-125">Safety stock quantity</span></span>
- <span data-ttu-id="dc595-126">Reorder point</span><span class="sxs-lookup"><span data-stu-id="dc595-126">Reorder point</span></span>
- <span data-ttu-id="dc595-127">Maximum inventory</span><span class="sxs-lookup"><span data-stu-id="dc595-127">Maximum inventory</span></span>
- <span data-ttu-id="dc595-128">Reorder quantity</span><span class="sxs-lookup"><span data-stu-id="dc595-128">Reorder quantity</span></span>
- <span data-ttu-id="dc595-129">Maximum order quantity</span><span class="sxs-lookup"><span data-stu-id="dc595-129">Maximum order quantity</span></span>
- <span data-ttu-id="dc595-130">Minimum order quantity</span><span class="sxs-lookup"><span data-stu-id="dc595-130">Minimum order quantity</span></span>
- <span data-ttu-id="dc595-131">Order multiple</span><span class="sxs-lookup"><span data-stu-id="dc595-131">Order multiple</span></span>
- <span data-ttu-id="dc595-132">Dampener (% of lot size)</span><span class="sxs-lookup"><span data-stu-id="dc595-132">Dampener (% of lot size)</span></span>

## <a name="see-also"></a><span data-ttu-id="dc595-133">See Also</span><span class="sxs-lookup"><span data-stu-id="dc595-133">See Also</span></span>  
[<span data-ttu-id="dc595-134">Planning</span><span class="sxs-lookup"><span data-stu-id="dc595-134">Planning</span></span>](production-planning.md)   
[<span data-ttu-id="dc595-135">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="dc595-135">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="dc595-136">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="dc595-136">Manufacturing</span></span>](production-manage-manufacturing.md)    
[<span data-ttu-id="dc595-137">Inventory</span><span class="sxs-lookup"><span data-stu-id="dc595-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="dc595-138">Purchasing</span><span class="sxs-lookup"><span data-stu-id="dc595-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="dc595-139">Design Details: Reservation, Tracking, and Action Messaging</span><span class="sxs-lookup"><span data-stu-id="dc595-139">Design Details: Reservation, Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="dc595-140">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="dc595-140">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)   
[<span data-ttu-id="dc595-141">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="dc595-141">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
[<span data-ttu-id="dc595-142">Working with</span><span class="sxs-lookup"><span data-stu-id="dc595-142">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
