---
title: How to Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal
description: You can use the **Applies-from Entry** field in the **Item Journal** window to create a fixed application between an inbound transaction and the original outbound transaction. For example, to correct the outbound transaction or to process its return.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/09/2017
ms.author: sgroespe
ms.openlocfilehash: 70d0e51a1f319b400dee175e6614d4a0444ff07a
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "6958"
---
# <a name="how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="692f4-104">How to: Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span><span class="sxs-lookup"><span data-stu-id="692f4-104">How to: Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>
<span data-ttu-id="692f4-105">You can use the **Applies-from Entry** field in the **Item Journal** window to create a fixed application between an inbound transaction and the original outbound transaction.</span><span class="sxs-lookup"><span data-stu-id="692f4-105">You can use the **Applies-from Entry** field in the **Item Journal** window to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="692f4-106">For example, to correct the outbound transaction or to process its return.</span><span class="sxs-lookup"><span data-stu-id="692f4-106">For example, to correct the outbound transaction or to process its return.</span></span> <span data-ttu-id="692f4-107">For more information, see Applies-from Entry.</span><span class="sxs-lookup"><span data-stu-id="692f4-107">For more information, see Applies-from Entry.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="692f4-108">Fixed applications made in this manner only apply the cost, not the quantity.</span><span class="sxs-lookup"><span data-stu-id="692f4-108">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="692f4-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span><span class="sxs-lookup"><span data-stu-id="692f4-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="692f4-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span><span class="sxs-lookup"><span data-stu-id="692f4-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>   
>  <span data-ttu-id="692f4-111">This also means that you cannot close an inventory period if such an entry exists.</span><span class="sxs-lookup"><span data-stu-id="692f4-111">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="692f4-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span><span class="sxs-lookup"><span data-stu-id="692f4-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="692f4-113">To close open item ledger entries that result from a fixed application in the item journal</span><span class="sxs-lookup"><span data-stu-id="692f4-113">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1.  <span data-ttu-id="692f4-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span><span class="sxs-lookup"><span data-stu-id="692f4-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="692f4-115">This closes the original negative entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="692f4-115">This closes the original negative entry with a fixed application.</span></span>  
2.  <span data-ttu-id="692f4-116">Use the **Applies-to Entry** field to post a negative adjustment.</span><span class="sxs-lookup"><span data-stu-id="692f4-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="692f4-117">This closes the original corrective positive entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="692f4-117">This closes the original corrective positive entry with a fixed application.</span></span>  

## <a name="see-also"></a><span data-ttu-id="692f4-118">See Also</span><span class="sxs-lookup"><span data-stu-id="692f4-118">See Also</span></span>  
[ <span data-ttu-id="692f4-119">How to: Remove and Reapply Item Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="692f4-119">How to: Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
 [<span data-ttu-id="692f4-120">How to: Process Sales Returns and Cancellations</span><span class="sxs-lookup"><span data-stu-id="692f4-120">How to: Process Sales Returns and Cancellations</span></span>](sales-how-process-sales-returns-cancellations.md)   
 [<span data-ttu-id="692f4-121">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="692f4-121">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)   
 [<span data-ttu-id="692f4-122">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="692f4-122">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)   
 [<span data-ttu-id="692f4-123">Design Details: Costing Methods</span><span class="sxs-lookup"><span data-stu-id="692f4-123">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)
