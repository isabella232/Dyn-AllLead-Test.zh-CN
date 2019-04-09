---
title: How to Set Up Cost Centers
description: Cost centers are departments that are responsible for costs and income. The chart of cost centers is similar to the dimension information for the general ledger.
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
ms.openlocfilehash: 2e22558e15e343a4a32520446dce0411fd3d44aa
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7166"
---
# <a name="how-to-set-up-cost-centers"></a><span data-ttu-id="f5a6e-104">How to: Set Up Cost Centers</span><span class="sxs-lookup"><span data-stu-id="f5a6e-104">How to: Set Up Cost Centers</span></span>
<span data-ttu-id="f5a6e-105">Cost centers are departments that are responsible for costs and income.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="f5a6e-106">The chart of cost centers is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="f5a6e-107">You can set up the chart of cost centers in the following ways:</span><span class="sxs-lookup"><span data-stu-id="f5a6e-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="f5a6e-108">Transfer dimension values in the general ledger to the chart of cost centers.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="f5a6e-109">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="f5a6e-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="f5a6e-111">You must create each cost center individually.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="f5a6e-112">To transfer dimension values in the general ledger to the chart of cost centers</span><span class="sxs-lookup"><span data-stu-id="f5a6e-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="f5a6e-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span></span> <span data-ttu-id="f5a6e-114">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="f5a6e-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="f5a6e-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="f5a6e-117">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f5a6e-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="f5a6e-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="f5a6e-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a><span data-ttu-id="f5a6e-121">To create new cost centers in the Chart of Cost Centers window</span><span class="sxs-lookup"><span data-stu-id="f5a6e-121">To create new cost centers in the Chart of Cost Centers window</span></span>  
<span data-ttu-id="f5a6e-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span></span> <span data-ttu-id="f5a6e-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span></span>  

1. <span data-ttu-id="f5a6e-124">Open the **Chart of Cost Centers** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-124">Open the **Chart of Cost Centers** window in edit mode.</span></span>  
2. <span data-ttu-id="f5a6e-125">In the **Code** field, enter the cost center code.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="f5a6e-126">All cost centers must have a code.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="f5a6e-127">In the **Name** field, enter the cost center name.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="f5a6e-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="f5a6e-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="f5a6e-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="f5a6e-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="f5a6e-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="f5a6e-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="f5a6e-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="f5a6e-135">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="f5a6e-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="f5a6e-137">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="f5a6e-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5a6e-138">See Also</span><span class="sxs-lookup"><span data-stu-id="f5a6e-138">See Also</span></span>  
[<span data-ttu-id="f5a6e-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="f5a6e-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
[<span data-ttu-id="f5a6e-140">Setting Up Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="f5a6e-140">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)   
[<span data-ttu-id="f5a6e-141">Terminology in Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="f5a6e-141">Terminology in Cost Accounting</span></span>](finance-terminology-in-cost-accounting.md)   
[<span data-ttu-id="f5a6e-142">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="f5a6e-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
[<span data-ttu-id="f5a6e-143">Working with</span><span class="sxs-lookup"><span data-stu-id="f5a6e-143">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
