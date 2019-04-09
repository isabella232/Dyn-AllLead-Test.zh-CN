---
title: Design Details - The Role of the Time Bucket
description: The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.
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
ms.openlocfilehash: d57b2611490af7c5f1737f30574cb80cfcddf4ca
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7182"
---
# <a name="design-details-the-role-of-the-time-bucket"></a><span data-ttu-id="9220c-103">Design Details: The Role of the Time Bucket</span><span class="sxs-lookup"><span data-stu-id="9220c-103">Design Details: The Role of the Time Bucket</span></span>
<span data-ttu-id="9220c-104">The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.</span><span class="sxs-lookup"><span data-stu-id="9220c-104">The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.</span></span>  
  
 <span data-ttu-id="9220c-105">For reordering policies that use a reorder point, you can define a time bucket.</span><span class="sxs-lookup"><span data-stu-id="9220c-105">For reordering policies that use a reorder point, you can define a time bucket.</span></span> <span data-ttu-id="9220c-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span><span class="sxs-lookup"><span data-stu-id="9220c-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span></span> <span data-ttu-id="9220c-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span><span class="sxs-lookup"><span data-stu-id="9220c-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span></span> <span data-ttu-id="9220c-108">The time buckets begin on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="9220c-108">The time buckets begin on the planning starting date.</span></span>  
  
 <span data-ttu-id="9220c-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span><span class="sxs-lookup"><span data-stu-id="9220c-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span></span> <span data-ttu-id="9220c-110">The user needs to define the frequency (the time bucket).</span><span class="sxs-lookup"><span data-stu-id="9220c-110">The user needs to define the frequency (the time bucket).</span></span> <span data-ttu-id="9220c-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span><span class="sxs-lookup"><span data-stu-id="9220c-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span></span>  
  
 <span data-ttu-id="9220c-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span><span class="sxs-lookup"><span data-stu-id="9220c-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span></span>  
  
 <span data-ttu-id="9220c-113">The time bucket is generally used to avoid a cascade effect.</span><span class="sxs-lookup"><span data-stu-id="9220c-113">The time bucket is generally used to avoid a cascade effect.</span></span> <span data-ttu-id="9220c-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span><span class="sxs-lookup"><span data-stu-id="9220c-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span></span> <span data-ttu-id="9220c-115">The result would be that every supply order (except the last one) is rescheduled.</span><span class="sxs-lookup"><span data-stu-id="9220c-115">The result would be that every supply order (except the last one) is rescheduled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="9220c-116">See Also</span><span class="sxs-lookup"><span data-stu-id="9220c-116">See Also</span></span>  
 [<span data-ttu-id="9220c-117">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="9220c-117">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)   
 [<span data-ttu-id="9220c-118">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="9220c-118">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)   
 [<span data-ttu-id="9220c-119">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="9220c-119">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)   
 [<span data-ttu-id="9220c-120">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="9220c-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)