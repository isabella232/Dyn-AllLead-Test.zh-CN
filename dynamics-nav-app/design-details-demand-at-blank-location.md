---
title: Design Details - Demand and Supply
description: This topic introduces the concept of demand, which is the common term used for any kind of gross demand, such as a sales order and component need from a production order.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 44481735b4eb326b9508155276736c59c1cfe516
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "6906"
---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="54031-103">Design Details: Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="54031-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="54031-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span><span class="sxs-lookup"><span data-stu-id="54031-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="54031-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span><span class="sxs-lookup"><span data-stu-id="54031-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="54031-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="54031-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="54031-107">In addition, a sales return may also represent supply.</span><span class="sxs-lookup"><span data-stu-id="54031-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="54031-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span><span class="sxs-lookup"><span data-stu-id="54031-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="54031-109">One profile holds demand events, and the other holds the corresponding supply events.</span><span class="sxs-lookup"><span data-stu-id="54031-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="54031-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span><span class="sxs-lookup"><span data-stu-id="54031-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="54031-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span><span class="sxs-lookup"><span data-stu-id="54031-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="54031-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span><span class="sxs-lookup"><span data-stu-id="54031-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="54031-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="54031-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="54031-114">See Also</span><span class="sxs-lookup"><span data-stu-id="54031-114">See Also</span></span>  
[<span data-ttu-id="54031-115">Design Details: Balancing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="54031-115">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)   
[<span data-ttu-id="54031-116">Design Details: Central Concepts of the Planning System</span><span class="sxs-lookup"><span data-stu-id="54031-116">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)   
[<span data-ttu-id="54031-117">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="54031-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)