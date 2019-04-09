---
title: Criteria for Transferring General Ledger Entries to Cost Entries
description: It is important to understand the criteria for transferring general ledger entries to cost entries. During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.
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
ms.openlocfilehash: f52ad05dcb23fd00a3c3fdb885759b08a6f2e72d
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7445"
---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="fc24f-104">Criteria for Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="fc24f-104">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="fc24f-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="fc24f-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="fc24f-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span><span class="sxs-lookup"><span data-stu-id="fc24f-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="fc24f-107">General ledger entries are transferred if:</span><span class="sxs-lookup"><span data-stu-id="fc24f-107">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="fc24f-108">The entries have dimension values corresponding to either a cost center or a cost object.</span><span class="sxs-lookup"><span data-stu-id="fc24f-108">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="fc24f-109">The entries have dimension values that correspond to a cost center and a cost object.</span><span class="sxs-lookup"><span data-stu-id="fc24f-109">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="fc24f-110">For these entries, the cost center takes precedence.</span><span class="sxs-lookup"><span data-stu-id="fc24f-110">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="fc24f-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span><span class="sxs-lookup"><span data-stu-id="fc24f-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="fc24f-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span><span class="sxs-lookup"><span data-stu-id="fc24f-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="fc24f-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span><span class="sxs-lookup"><span data-stu-id="fc24f-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="fc24f-114">General ledger entries are not transferred if:</span><span class="sxs-lookup"><span data-stu-id="fc24f-114">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="fc24f-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span><span class="sxs-lookup"><span data-stu-id="fc24f-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="fc24f-116">The entries have an amount of zero.</span><span class="sxs-lookup"><span data-stu-id="fc24f-116">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="fc24f-117">The entries have a general ledger account that has been deleted.</span><span class="sxs-lookup"><span data-stu-id="fc24f-117">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="fc24f-118">The entries have a general ledger account that is not of the type **Income Statement**.</span><span class="sxs-lookup"><span data-stu-id="fc24f-118">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="fc24f-119">The entries have a general ledger account that is not assigned a cost type.</span><span class="sxs-lookup"><span data-stu-id="fc24f-119">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="fc24f-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span><span class="sxs-lookup"><span data-stu-id="fc24f-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="fc24f-121">The entries have been posted with a closing date.</span><span class="sxs-lookup"><span data-stu-id="fc24f-121">The entries have been posted with a closing date.</span></span> <span data-ttu-id="fc24f-122">These are typically entries that set back the balance of the income statement at the end of the year.</span><span class="sxs-lookup"><span data-stu-id="fc24f-122">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc24f-123">See Also</span><span class="sxs-lookup"><span data-stu-id="fc24f-123">See Also</span></span>  
[<span data-ttu-id="fc24f-124">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="fc24f-124">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 [<span data-ttu-id="fc24f-125">How to: Transfer General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="fc24f-125">How to: Transfer General Ledger Entries to Cost Entries</span></span>](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [<span data-ttu-id="fc24f-126">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="fc24f-126">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)   
 [<span data-ttu-id="fc24f-127">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="fc24f-127">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
 [<span data-ttu-id="fc24f-128">Working with</span><span class="sxs-lookup"><span data-stu-id="fc24f-128">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
