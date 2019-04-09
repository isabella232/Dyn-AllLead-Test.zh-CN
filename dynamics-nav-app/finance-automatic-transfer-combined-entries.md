---
title: Automatic Transfer and Combined Entries
description: In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting. You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition. The following table describes the different options.
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
ms.openlocfilehash: c00295dfdcd0d1da63b33b8379079fcb91ac33ec
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7250"
---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="8f683-105">Automatic Transfer and Combined Entries</span><span class="sxs-lookup"><span data-stu-id="8f683-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="8f683-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span><span class="sxs-lookup"><span data-stu-id="8f683-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="8f683-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span><span class="sxs-lookup"><span data-stu-id="8f683-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="8f683-108">The following table describes the different options.</span><span class="sxs-lookup"><span data-stu-id="8f683-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="8f683-109">Combine entries</span><span class="sxs-lookup"><span data-stu-id="8f683-109">Combine entries</span></span>|<span data-ttu-id="8f683-110">Description</span><span class="sxs-lookup"><span data-stu-id="8f683-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="8f683-111">None</span><span class="sxs-lookup"><span data-stu-id="8f683-111">None</span></span>|<span data-ttu-id="8f683-112">Each general ledger entry is transferred individually to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="8f683-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="8f683-113">Day</span><span class="sxs-lookup"><span data-stu-id="8f683-113">Day</span></span>|<span data-ttu-id="8f683-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="8f683-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="8f683-115">Month</span><span class="sxs-lookup"><span data-stu-id="8f683-115">Month</span></span>|<span data-ttu-id="8f683-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="8f683-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="8f683-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="8f683-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="8f683-118">Combined entries are not possible.</span><span class="sxs-lookup"><span data-stu-id="8f683-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8f683-119">See Also</span><span class="sxs-lookup"><span data-stu-id="8f683-119">See Also</span></span>  
 [<span data-ttu-id="8f683-120">How to: Transfer General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="8f683-120">How to: Transfer General Ledger Entries to Cost Entries</span></span>](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [<span data-ttu-id="8f683-121">Criteria for Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="8f683-121">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [<span data-ttu-id="8f683-122">Results of the Transfer</span><span class="sxs-lookup"><span data-stu-id="8f683-122">Results of the Transfer</span></span>](finance-results-of-the-transfer.md)   
 [<span data-ttu-id="8f683-123">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="8f683-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 [<span data-ttu-id="8f683-124">Working with</span><span class="sxs-lookup"><span data-stu-id="8f683-124">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
