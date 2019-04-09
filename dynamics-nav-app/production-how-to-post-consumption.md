---
title: How to Batch Post Consumption
description: If the flushing method is **Manual**, you must post the components manually, using a consumption journal.
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
ms.openlocfilehash: df466b9d00894c28a5ea72a720093bf69443473e
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7487"
---
# <a name="how-to-batch-post-production-consumption"></a><span data-ttu-id="74fa7-103">How to: Batch Post Production Consumption</span><span class="sxs-lookup"><span data-stu-id="74fa7-103">How to: Batch Post Production Consumption</span></span>
<span data-ttu-id="74fa7-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span><span class="sxs-lookup"><span data-stu-id="74fa7-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="74fa7-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span><span class="sxs-lookup"><span data-stu-id="74fa7-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="74fa7-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="74fa7-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="74fa7-107">To post consumption for one or more production order lines</span><span class="sxs-lookup"><span data-stu-id="74fa7-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="74fa7-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="74fa7-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="74fa7-109">Fill in the fields with the production order data and the consumption data.</span><span class="sxs-lookup"><span data-stu-id="74fa7-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="74fa7-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="74fa7-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="74fa7-111">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="74fa7-111">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="74fa7-112">Choose the **Post** action to post the consumption.</span><span class="sxs-lookup"><span data-stu-id="74fa7-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="74fa7-113">The related item ledger entries are reduced.</span><span class="sxs-lookup"><span data-stu-id="74fa7-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="74fa7-114">See Also</span><span class="sxs-lookup"><span data-stu-id="74fa7-114">See Also</span></span>  
[<span data-ttu-id="74fa7-115">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="74fa7-115">Manufacturing</span></span>](production-manage-manufacturing.md)    
[<span data-ttu-id="74fa7-116">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="74fa7-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="74fa7-117">Planning</span><span class="sxs-lookup"><span data-stu-id="74fa7-117">Planning</span></span>](production-planning.md)      
[<span data-ttu-id="74fa7-118">Inventory</span><span class="sxs-lookup"><span data-stu-id="74fa7-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="74fa7-119">Purchasing</span><span class="sxs-lookup"><span data-stu-id="74fa7-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="74fa7-120">Working with</span><span class="sxs-lookup"><span data-stu-id="74fa7-120">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
