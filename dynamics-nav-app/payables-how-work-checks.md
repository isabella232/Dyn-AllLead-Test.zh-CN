---
title: Issue, Print, Cancel, and Void Checks
description: Describes how to issue checks using the payment journal, print checks, and void or view check ledger entries in Dynamics NAV.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.openlocfilehash: e6da9fd8802bee0c8fb3632fb95d38da63d20c7b
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7244"
---
# <a name="how-to-work-with-checks"></a><span data-ttu-id="ee788-103">How to: Work With Checks</span><span class="sxs-lookup"><span data-stu-id="ee788-103">How to: Work With Checks</span></span>
<span data-ttu-id="ee788-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ee788-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="ee788-105">Both methods use the payment journal to issue checks to vendors.</span><span class="sxs-lookup"><span data-stu-id="ee788-105">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="ee788-106">You can also void checks and view check ledger entries.</span><span class="sxs-lookup"><span data-stu-id="ee788-106">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="ee788-107">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span><span class="sxs-lookup"><span data-stu-id="ee788-107">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ee788-108">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span><span class="sxs-lookup"><span data-stu-id="ee788-108">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span></span> <span data-ttu-id="ee788-109">For more information, see [How to: Export a Positive Pay file](finance-how-positive-pay.md).</span><span class="sxs-lookup"><span data-stu-id="ee788-109">For more information, see [How to: Export a Positive Pay file](finance-how-positive-pay.md).</span></span>

<span data-ttu-id="ee788-110">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span><span class="sxs-lookup"><span data-stu-id="ee788-110">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="ee788-111">For more information, see [How to: Define Check Layouts](finance-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="ee788-111">For more information, see [How to: Define Check Layouts](finance-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="ee788-112">To issue checks</span><span class="sxs-lookup"><span data-stu-id="ee788-112">To issue checks</span></span>
1. <span data-ttu-id="ee788-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ee788-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="ee788-114">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span><span class="sxs-lookup"><span data-stu-id="ee788-114">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="ee788-115">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="ee788-115">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="ee788-116">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="ee788-116">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

   * <span data-ttu-id="ee788-117">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span><span class="sxs-lookup"><span data-stu-id="ee788-117">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="ee788-118">You must print the checks before you can post the journal lines.</span><span class="sxs-lookup"><span data-stu-id="ee788-118">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="ee788-119">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="ee788-119">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>
   * <span data-ttu-id="ee788-120">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span><span class="sxs-lookup"><span data-stu-id="ee788-120">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="ee788-121">By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ee788-121">By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="ee788-122">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="ee788-122">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

     > [!NOTE]  
     >   <span data-ttu-id="ee788-123">You must print computer checks before you post the related journal lines.</span><span class="sxs-lookup"><span data-stu-id="ee788-123">You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="ee788-124">In case of computer checks, choose **Print Check**.</span><span class="sxs-lookup"><span data-stu-id="ee788-124">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="ee788-125">In the **Check** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ee788-125">In the **Check** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
6. <span data-ttu-id="ee788-126">Choose the **Print** button.</span><span class="sxs-lookup"><span data-stu-id="ee788-126">Choose the **Print** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ee788-127">If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span><span class="sxs-lookup"><span data-stu-id="ee788-127">If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="ee788-128">To cancel printed checks that are not posted</span><span class="sxs-lookup"><span data-stu-id="ee788-128">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="ee788-129">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="ee788-129">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>

1. <span data-ttu-id="ee788-130">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span><span class="sxs-lookup"><span data-stu-id="ee788-130">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="ee788-131">To void checks</span><span class="sxs-lookup"><span data-stu-id="ee788-131">To void checks</span></span>
<span data-ttu-id="ee788-132">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span><span class="sxs-lookup"><span data-stu-id="ee788-132">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="ee788-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ee788-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ee788-134">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="ee788-134">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="ee788-135">In the **Check Ledger Entries** window, choose the **Void Check** action.</span><span class="sxs-lookup"><span data-stu-id="ee788-135">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="ee788-136">Select the **Void Check Only** check box.</span><span class="sxs-lookup"><span data-stu-id="ee788-136">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="ee788-137">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="ee788-137">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="ee788-138">See Also</span><span class="sxs-lookup"><span data-stu-id="ee788-138">See Also</span></span>
[<span data-ttu-id="ee788-139">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="ee788-139">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="ee788-140">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="ee788-140">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="ee788-141">How to: Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="ee788-141">How to: Export a Positive Pay file</span></span>](finance-how-positive-pay.md)  
[<span data-ttu-id="ee788-142">Working with</span><span class="sxs-lookup"><span data-stu-id="ee788-142">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
