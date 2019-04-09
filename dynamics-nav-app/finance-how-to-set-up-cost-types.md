---
title: How to Set Up a Chart of Cost Types
description: Chart of cost types are similar to the chart of accounts in the general ledger.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger, accounts
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 87586e4f023fc7c07aa0e41889046e79d7e26fb6
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7410"
---
# <a name="how-to-set-up-cost-types"></a><span data-ttu-id="66ad9-103">How to: Set Up Cost Types</span><span class="sxs-lookup"><span data-stu-id="66ad9-103">How to: Set Up Cost Types</span></span>
<span data-ttu-id="66ad9-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="66ad9-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span></span> <span data-ttu-id="66ad9-105">You can set up the chart of cost types in the following ways:</span><span class="sxs-lookup"><span data-stu-id="66ad9-105">You can set up the chart of cost types in the following ways:</span></span>  

-   <span data-ttu-id="66ad9-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="66ad9-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span></span> <span data-ttu-id="66ad9-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="66ad9-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span></span> <span data-ttu-id="66ad9-108">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="66ad9-108">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="66ad9-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="66ad9-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span></span> <span data-ttu-id="66ad9-110">You must create each new cost type individually.</span><span class="sxs-lookup"><span data-stu-id="66ad9-110">You must create each new cost type individually.</span></span>  

## <a name="to-transfer-the-general-ledger-chart-of-accounts-to-the-chart-of-cost-types"></a><span data-ttu-id="66ad9-111">To transfer the general ledger chart of accounts to the chart of cost types</span><span class="sxs-lookup"><span data-stu-id="66ad9-111">To transfer the general ledger chart of accounts to the chart of cost types</span></span>  
1.  <span data-ttu-id="66ad9-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="66ad9-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="66ad9-113">Choose the **Get Cost Types from Chart of Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="66ad9-113">Choose the **Get Cost Types from Chart of Accounts** action.</span></span> <span data-ttu-id="66ad9-114">In the dialog box, choose the **Yes** button to confirm the transfer.</span><span class="sxs-lookup"><span data-stu-id="66ad9-114">In the dialog box, choose the **Yes** button to confirm the transfer.</span></span> <span data-ttu-id="66ad9-115">The function uses the chart of accounts to create a chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="66ad9-115">The function uses the chart of accounts to create a chart of cost types.</span></span>  

    <span data-ttu-id="66ad9-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span><span class="sxs-lookup"><span data-stu-id="66ad9-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span></span> <span data-ttu-id="66ad9-117">You can change the chart of cost types, as necessary.</span><span class="sxs-lookup"><span data-stu-id="66ad9-117">You can change the chart of cost types, as necessary.</span></span> <span data-ttu-id="66ad9-118">For example, you can delete duplicate existing cost types.</span><span class="sxs-lookup"><span data-stu-id="66ad9-118">For example, you can delete duplicate existing cost types.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="66ad9-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="66ad9-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span></span> <span data-ttu-id="66ad9-120">The **No.**</span><span class="sxs-lookup"><span data-stu-id="66ad9-120">The **No.**</span></span> <span data-ttu-id="66ad9-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="66ad9-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span></span> <span data-ttu-id="66ad9-122">The function runs automatically before transferring general ledger entries to cost accounting.</span><span class="sxs-lookup"><span data-stu-id="66ad9-122">The function runs automatically before transferring general ledger entries to cost accounting.</span></span>  

## <a name="to-set-up-new-cost-types-in-the-chart-of-cost-types-window"></a><span data-ttu-id="66ad9-123">To set up new cost types in the Chart of Cost Types window</span><span class="sxs-lookup"><span data-stu-id="66ad9-123">To set up new cost types in the Chart of Cost Types window</span></span>  
1.  <span data-ttu-id="66ad9-124">Open the **Chart of Cost Types** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="66ad9-124">Open the **Chart of Cost Types** window in edit mode.</span></span>  
2.  <span data-ttu-id="66ad9-125">Fill in the fields as described as necessary.</span><span class="sxs-lookup"><span data-stu-id="66ad9-125">Fill in the fields as described as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >  <span data-ttu-id="66ad9-126">You can set up and maintain cost types in either the **Cost Type Card** window or in the **Chart of Cost Types** window.</span><span class="sxs-lookup"><span data-stu-id="66ad9-126">You can set up and maintain cost types in either the **Cost Type Card** window or in the **Chart of Cost Types** window.</span></span> <span data-ttu-id="66ad9-127">In this procedure, you set up cost types in the **Chart of Cost Types** window.</span><span class="sxs-lookup"><span data-stu-id="66ad9-127">In this procedure, you set up cost types in the **Chart of Cost Types** window.</span></span>

3.  <span data-ttu-id="66ad9-128">After you have created all cost types, choose the **Indent Cost Types** action.</span><span class="sxs-lookup"><span data-stu-id="66ad9-128">After you have created all cost types, choose the **Indent Cost Types** action.</span></span> <span data-ttu-id="66ad9-129">In the dialog box, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="66ad9-129">In the dialog box, choose the **Yes** button.</span></span>  
4.  <span data-ttu-id="66ad9-130">Link the new cost type to the corresponding general ledger account.</span><span class="sxs-lookup"><span data-stu-id="66ad9-130">Link the new cost type to the corresponding general ledger account.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="66ad9-131">If you have entered definitions in the **Totaling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="66ad9-131">If you have entered definitions in the **Totaling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="to-update-cost-types"></a><span data-ttu-id="66ad9-132">To update cost types</span><span class="sxs-lookup"><span data-stu-id="66ad9-132">To update cost types</span></span>  
1.  <span data-ttu-id="66ad9-133">In the **Cost Accounting Setup** window, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span><span class="sxs-lookup"><span data-stu-id="66ad9-133">In the **Cost Accounting Setup** window, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span></span>  
2.  <span data-ttu-id="66ad9-134">In the **Align G/L Account** field, you can choose from the following options.</span><span class="sxs-lookup"><span data-stu-id="66ad9-134">In the **Align G/L Account** field, you can choose from the following options.</span></span>  

- <span data-ttu-id="66ad9-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="66ad9-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="66ad9-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="66ad9-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="66ad9-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="66ad9-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="66ad9-138">See Also</span><span class="sxs-lookup"><span data-stu-id="66ad9-138">See Also</span></span>  
[<span data-ttu-id="66ad9-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="66ad9-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
[<span data-ttu-id="66ad9-140">Defining the Relationship Between Cost Types and General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="66ad9-140">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   
[<span data-ttu-id="66ad9-141">Defining Cost Centers and Cost Objects for Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="66ad9-141">Defining Cost Centers and Cost Objects for Chart of Accounts</span></span>](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md)   
[<span data-ttu-id="66ad9-142">Balances Between Cost Type, Cost Center, and Cost Object</span><span class="sxs-lookup"><span data-stu-id="66ad9-142">Balances Between Cost Type, Cost Center, and Cost Object</span></span>](finance-balances-between-cost-type-cost-center-and-cost-object.md)   
[<span data-ttu-id="66ad9-143">Setting Up Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="66ad9-143">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)   
[<span data-ttu-id="66ad9-144">Terminology in Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="66ad9-144">Terminology in Cost Accounting</span></span>](finance-terminology-in-cost-accounting.md)   
[<span data-ttu-id="66ad9-145">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="66ad9-145">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
[<span data-ttu-id="66ad9-146">Working with</span><span class="sxs-lookup"><span data-stu-id="66ad9-146">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
