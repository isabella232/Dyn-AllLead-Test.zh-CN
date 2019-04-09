---
title: Design Details - Closing Demand and Supply
description: When the supply balancing procedures have been performed, there are three possible end situations.
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
ms.openlocfilehash: c6a08676e8e467d1c66e9bbcae51161ce89fda14
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7443"
---
# <a name="design-details-closing-demand-and-supply"></a><span data-ttu-id="fc789-103">Design Details: Closing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="fc789-103">Design Details: Closing Demand and Supply</span></span>
<span data-ttu-id="fc789-104">When the supply balancing procedures have been performed, there are three possible end situations:</span><span class="sxs-lookup"><span data-stu-id="fc789-104">When the supply balancing procedures have been performed, there are three possible end situations:</span></span>  

- <span data-ttu-id="fc789-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span><span class="sxs-lookup"><span data-stu-id="fc789-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span></span> <span data-ttu-id="fc789-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span><span class="sxs-lookup"><span data-stu-id="fc789-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span></span>  

- <span data-ttu-id="fc789-107">The supply order cannot be modified to cover all of the demand.</span><span class="sxs-lookup"><span data-stu-id="fc789-107">The supply order cannot be modified to cover all of the demand.</span></span> <span data-ttu-id="fc789-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span><span class="sxs-lookup"><span data-stu-id="fc789-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span></span> <span data-ttu-id="fc789-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span><span class="sxs-lookup"><span data-stu-id="fc789-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span></span>  

- <span data-ttu-id="fc789-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span><span class="sxs-lookup"><span data-stu-id="fc789-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span></span> <span data-ttu-id="fc789-111">If there is any surplus supply, it may be decreased (or canceled) and then closed.</span><span class="sxs-lookup"><span data-stu-id="fc789-111">If there is any surplus supply, it may be decreased (or canceled) and then closed.</span></span> <span data-ttu-id="fc789-112">It is possible that additional supply events exist further along in the chain, and they should also be canceled.</span><span class="sxs-lookup"><span data-stu-id="fc789-112">It is possible that additional supply events exist further along in the chain, and they should also be canceled.</span></span>  

  <span data-ttu-id="fc789-113">Last, the planning system will create an order tracking link between the supply and the demand.</span><span class="sxs-lookup"><span data-stu-id="fc789-113">Last, the planning system will create an order tracking link between the supply and the demand.</span></span>  

## <a name="creating-the-planning-line-suggested-action"></a><span data-ttu-id="fc789-114">Creating the Planning Line (Suggested Action)</span><span class="sxs-lookup"><span data-stu-id="fc789-114">Creating the Planning Line (Suggested Action)</span></span>  
 <span data-ttu-id="fc789-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span><span class="sxs-lookup"><span data-stu-id="fc789-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span></span> <span data-ttu-id="fc789-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span><span class="sxs-lookup"><span data-stu-id="fc789-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span></span> <span data-ttu-id="fc789-117">This means that when first created, the planning line may be changed again.</span><span class="sxs-lookup"><span data-stu-id="fc789-117">This means that when first created, the planning line may be changed again.</span></span>  

 <span data-ttu-id="fc789-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span><span class="sxs-lookup"><span data-stu-id="fc789-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span></span>  

- <span data-ttu-id="fc789-119">Create only the planning line with the current due date and quantity but without the routing and components.</span><span class="sxs-lookup"><span data-stu-id="fc789-119">Create only the planning line with the current due date and quantity but without the routing and components.</span></span>  

- <span data-ttu-id="fc789-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span><span class="sxs-lookup"><span data-stu-id="fc789-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span></span> <span data-ttu-id="fc789-121">This is demanding in terms of database accesses.</span><span class="sxs-lookup"><span data-stu-id="fc789-121">This is demanding in terms of database accesses.</span></span> <span data-ttu-id="fc789-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span><span class="sxs-lookup"><span data-stu-id="fc789-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span></span>  

- <span data-ttu-id="fc789-123">Include BOM explosion: this can wait until just before the supply event is closed.</span><span class="sxs-lookup"><span data-stu-id="fc789-123">Include BOM explosion: this can wait until just before the supply event is closed.</span></span>  

  <span data-ttu-id="fc789-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span><span class="sxs-lookup"><span data-stu-id="fc789-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span></span> <span data-ttu-id="fc789-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span><span class="sxs-lookup"><span data-stu-id="fc789-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc789-126">See Also</span><span class="sxs-lookup"><span data-stu-id="fc789-126">See Also</span></span>  
 [<span data-ttu-id="fc789-127">Design Details: Balancing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="fc789-127">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)   
 [<span data-ttu-id="fc789-128">Design Details: Central Concepts of the Planning System</span><span class="sxs-lookup"><span data-stu-id="fc789-128">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)   
 [<span data-ttu-id="fc789-129">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="fc789-129">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
