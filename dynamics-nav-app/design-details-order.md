---
title: Design Details - Order
description: This topic provides information about order-to-order links in a make-to-order environment.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, order
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: f1d2308a7adc89e8474384e3dffeab10345efa6f
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7527"
---
# <a name="design-details-order"></a><span data-ttu-id="d5d04-103">Design Details: Order</span><span class="sxs-lookup"><span data-stu-id="d5d04-103">Design Details: Order</span></span>
<span data-ttu-id="d5d04-104">In a make-to-order environment, an item is purchased or produced to exclusively cover a specific demand.</span><span class="sxs-lookup"><span data-stu-id="d5d04-104">In a make-to-order environment, an item is purchased or produced to exclusively cover a specific demand.</span></span> <span data-ttu-id="d5d04-105">Typically it relates to A-items, and the motivation for choosing the order reordering policy can be that the demand is infrequent, the lead-time is insignificant, or the required attributes vary.</span><span class="sxs-lookup"><span data-stu-id="d5d04-105">Typically it relates to A-items, and the motivation for choosing the order reordering policy can be that the demand is infrequent, the lead-time is insignificant, or the required attributes vary.</span></span>  
  
<span data-ttu-id="d5d04-106">The program creates an order-to-order link, which acts as a preliminary connection between the supply, a supply order or inventory, and the demand that it is going to fulfill.</span><span class="sxs-lookup"><span data-stu-id="d5d04-106">The program creates an order-to-order link, which acts as a preliminary connection between the supply, a supply order or inventory, and the demand that it is going to fulfill.</span></span>  
  
<span data-ttu-id="d5d04-107">Apart from using the Order policy, the order-to-order link can be applied during planning in the following ways:</span><span class="sxs-lookup"><span data-stu-id="d5d04-107">Apart from using the Order policy, the order-to-order link can be applied during planning in the following ways:</span></span>  
  
* <span data-ttu-id="d5d04-108">When using the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order).</span><span class="sxs-lookup"><span data-stu-id="d5d04-108">When using the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order).</span></span>  
* <span data-ttu-id="d5d04-109">When using the Sales Order Planning feature to create a production order from a sales order.</span><span class="sxs-lookup"><span data-stu-id="d5d04-109">When using the Sales Order Planning feature to create a production order from a sales order.</span></span>  
  
<span data-ttu-id="d5d04-110">Even if a manufacturing company considers itself as a make-to-order environment, it might be best to use a Lot-for-Lot reordering policy if the items are pure standard without variation in attributes.</span><span class="sxs-lookup"><span data-stu-id="d5d04-110">Even if a manufacturing company considers itself as a make-to-order environment, it might be best to use a Lot-for-Lot reordering policy if the items are pure standard without variation in attributes.</span></span> <span data-ttu-id="d5d04-111">As a result, the system will use unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.</span><span class="sxs-lookup"><span data-stu-id="d5d04-111">As a result, the system will use unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.</span></span>  
  
## <a name="order-to-order-links-and-past-due-dates"></a><span data-ttu-id="d5d04-112">Order-to-Order Links and Past Due Dates</span><span class="sxs-lookup"><span data-stu-id="d5d04-112">Order-to-Order Links and Past Due Dates</span></span>  
<span data-ttu-id="d5d04-113">Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system.</span><span class="sxs-lookup"><span data-stu-id="d5d04-113">Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system.</span></span> <span data-ttu-id="d5d04-114">The business reason for this exception is that specific demand-supply sets must be synchronized through to execution.</span><span class="sxs-lookup"><span data-stu-id="d5d04-114">The business reason for this exception is that specific demand-supply sets must be synchronized through to execution.</span></span> <span data-ttu-id="d5d04-115">For more information about the frozen zone that applies to most demand-supply types, see [Design Details: Dealing with Orders Before the Planning Starting Date](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span><span class="sxs-lookup"><span data-stu-id="d5d04-115">For more information about the frozen zone that applies to most demand-supply types, see [Design Details: Dealing with Orders Before the Planning Starting Date](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d5d04-116">See Also</span><span class="sxs-lookup"><span data-stu-id="d5d04-116">See Also</span></span>  
[<span data-ttu-id="d5d04-117">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="d5d04-117">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)   
[<span data-ttu-id="d5d04-118">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="d5d04-118">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)   
[<span data-ttu-id="d5d04-119">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="d5d04-119">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)   
[<span data-ttu-id="d5d04-120">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="d5d04-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)