---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules
description: This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/01/2017
ms.author: sgroespe
ms.openlocfilehash: a9c65032ab416809fa14b2b8a1149636c0571728
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7473"
---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a><span data-ttu-id="c76d4-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span><span class="sxs-lookup"><span data-stu-id="c76d4-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span></span>
<span data-ttu-id="c76d4-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="c76d4-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span></span> <span data-ttu-id="c76d4-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span><span class="sxs-lookup"><span data-stu-id="c76d4-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span></span> <span data-ttu-id="c76d4-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span><span class="sxs-lookup"><span data-stu-id="c76d4-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span></span> <span data-ttu-id="c76d4-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="c76d4-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="c76d4-111">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="c76d4-111">About This Walkthrough</span></span>  
<span data-ttu-id="c76d4-112">This walkthrough describes the following tasks:</span><span class="sxs-lookup"><span data-stu-id="c76d4-112">This walkthrough describes the following tasks:</span></span>  

- <span data-ttu-id="c76d4-113">Setting up a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="c76d4-113">Setting up a new cash flow account schedule name.</span></span>  
- <span data-ttu-id="c76d4-114">Setting up account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="c76d4-114">Setting up account schedule lines.</span></span>  
- <span data-ttu-id="c76d4-115">Setting up a new column layout.</span><span class="sxs-lookup"><span data-stu-id="c76d4-115">Setting up a new column layout.</span></span>  
- <span data-ttu-id="c76d4-116">Assigning a column layout to an account schedule.</span><span class="sxs-lookup"><span data-stu-id="c76d4-116">Assigning a column layout to an account schedule.</span></span>  
- <span data-ttu-id="c76d4-117">Viewing and printing the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="c76d4-117">Viewing and printing the cash flow forecast.</span></span>  

### <a name="prerequisites"></a><span data-ttu-id="c76d4-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="c76d4-118">Prerequisites</span></span>  
<span data-ttu-id="c76d4-119">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="c76d4-119">To complete this walkthrough, you will need:</span></span>  

- [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="c76d4-120">installed.</span><span class="sxs-lookup"><span data-stu-id="c76d4-120">installed.</span></span>  
- <span data-ttu-id="c76d4-121">The cash flow worksheet lines are registered.</span><span class="sxs-lookup"><span data-stu-id="c76d4-121">The cash flow worksheet lines are registered.</span></span>  

## <a name="roles"></a><span data-ttu-id="c76d4-122">Roles</span><span class="sxs-lookup"><span data-stu-id="c76d4-122">Roles</span></span>  
<span data-ttu-id="c76d4-123">This walkthrough demonstrates tasks that are performed by the following user role:</span><span class="sxs-lookup"><span data-stu-id="c76d4-123">This walkthrough demonstrates tasks that are performed by the following user role:</span></span>  

- <span data-ttu-id="c76d4-124">Controller</span><span class="sxs-lookup"><span data-stu-id="c76d4-124">Controller</span></span>  

## <a name="story"></a><span data-ttu-id="c76d4-125">Story</span><span class="sxs-lookup"><span data-stu-id="c76d4-125">Story</span></span>  
<span data-ttu-id="c76d4-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="c76d4-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span></span> <span data-ttu-id="c76d4-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span><span class="sxs-lookup"><span data-stu-id="c76d4-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span></span>  

## <a name="setting-up-a-new-account-schedule-name"></a><span data-ttu-id="c76d4-128">Setting Up a New Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="c76d4-128">Setting Up a New Account Schedule Name</span></span>  
<span data-ttu-id="c76d4-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span><span class="sxs-lookup"><span data-stu-id="c76d4-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span></span>  

### <a name="to-set-up-a-new-account-schedule-name"></a><span data-ttu-id="c76d4-130">To set up a new account schedule name</span><span class="sxs-lookup"><span data-stu-id="c76d4-130">To set up a new account schedule name</span></span>  

1.  <span data-ttu-id="c76d4-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c76d4-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c76d4-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="c76d4-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span></span>  
3.  <span data-ttu-id="c76d4-133">In the **Name** field, enter **Forecast**.</span><span class="sxs-lookup"><span data-stu-id="c76d4-133">In the **Name** field, enter **Forecast**.</span></span>  
4.  <span data-ttu-id="c76d4-134">In the **Description** field, enter **Cash Flow Forecast**.</span><span class="sxs-lookup"><span data-stu-id="c76d4-134">In the **Description** field, enter **Cash Flow Forecast**.</span></span>  
5.  <span data-ttu-id="c76d4-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span><span class="sxs-lookup"><span data-stu-id="c76d4-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span></span>  

## <a name="setting-up-account-schedule-lines"></a><span data-ttu-id="c76d4-136">Setting Up Account Schedule Lines</span><span class="sxs-lookup"><span data-stu-id="c76d4-136">Setting Up Account Schedule Lines</span></span>  
<span data-ttu-id="c76d4-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span><span class="sxs-lookup"><span data-stu-id="c76d4-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span></span> <span data-ttu-id="c76d4-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span><span class="sxs-lookup"><span data-stu-id="c76d4-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span></span>  

### <a name="to-set-up-account-schedule-lines"></a><span data-ttu-id="c76d4-139">To set up account schedule lines</span><span class="sxs-lookup"><span data-stu-id="c76d4-139">To set up account schedule lines</span></span>  

1. <span data-ttu-id="c76d4-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span><span class="sxs-lookup"><span data-stu-id="c76d4-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span></span> <span data-ttu-id="c76d4-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span><span class="sxs-lookup"><span data-stu-id="c76d4-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span></span>  
2. <span data-ttu-id="c76d4-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span><span class="sxs-lookup"><span data-stu-id="c76d4-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span></span>  

   > [!NOTE]  
   >  <span data-ttu-id="c76d4-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="c76d4-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span></span>  

   | <span data-ttu-id="c76d4-144">Row No.</span><span class="sxs-lookup"><span data-stu-id="c76d4-144">Row No.</span></span> |    <span data-ttu-id="c76d4-145">Description</span><span class="sxs-lookup"><span data-stu-id="c76d4-145">Description</span></span>     |   <span data-ttu-id="c76d4-146">Totaling Type</span><span class="sxs-lookup"><span data-stu-id="c76d4-146">Totaling Type</span></span>    | <span data-ttu-id="c76d4-147">Totaling</span><span class="sxs-lookup"><span data-stu-id="c76d4-147">Totaling</span></span> |  <span data-ttu-id="c76d4-148">Row Type</span><span class="sxs-lookup"><span data-stu-id="c76d4-148">Row Type</span></span>  | <span data-ttu-id="c76d4-149">Amount Type</span><span class="sxs-lookup"><span data-stu-id="c76d4-149">Amount Type</span></span> | <span data-ttu-id="c76d4-150">Show</span><span class="sxs-lookup"><span data-stu-id="c76d4-150">Show</span></span> |
   |---------|--------------------|--------------------|----------|------------|-------------|------|
   |   <span data-ttu-id="c76d4-151">C10</span><span class="sxs-lookup"><span data-stu-id="c76d4-151">C10</span></span>   |       <span data-ttu-id="c76d4-152">Amount</span><span class="sxs-lookup"><span data-stu-id="c76d4-152">Amount</span></span>       |     <span data-ttu-id="c76d4-153">Net Change</span><span class="sxs-lookup"><span data-stu-id="c76d4-153">Net Change</span></span>     | <span data-ttu-id="c76d4-154">Entries</span><span class="sxs-lookup"><span data-stu-id="c76d4-154">Entries</span></span>  | <span data-ttu-id="c76d4-155">Net Amount</span><span class="sxs-lookup"><span data-stu-id="c76d4-155">Net Amount</span></span> |   <span data-ttu-id="c76d4-156">Always</span><span class="sxs-lookup"><span data-stu-id="c76d4-156">Always</span></span>    |      |
   |   <span data-ttu-id="c76d4-157">C20</span><span class="sxs-lookup"><span data-stu-id="c76d4-157">C20</span></span>   | <span data-ttu-id="c76d4-158">Amount until Date</span><span class="sxs-lookup"><span data-stu-id="c76d4-158">Amount until Date</span></span>  |  <span data-ttu-id="c76d4-159">Balance at Date</span><span class="sxs-lookup"><span data-stu-id="c76d4-159">Balance at Date</span></span>   | <span data-ttu-id="c76d4-160">Entries</span><span class="sxs-lookup"><span data-stu-id="c76d4-160">Entries</span></span>  | <span data-ttu-id="c76d4-161">Net Amount</span><span class="sxs-lookup"><span data-stu-id="c76d4-161">Net Amount</span></span> |   <span data-ttu-id="c76d4-162">Always</span><span class="sxs-lookup"><span data-stu-id="c76d4-162">Always</span></span>    |      |
   |   <span data-ttu-id="c76d4-163">C30</span><span class="sxs-lookup"><span data-stu-id="c76d4-163">C30</span></span>   | <span data-ttu-id="c76d4-164">Entire Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="c76d4-164">Entire Fiscal Year</span></span> | <span data-ttu-id="c76d4-165">Entire Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="c76d4-165">Entire Fiscal Year</span></span> | <span data-ttu-id="c76d4-166">Entries</span><span class="sxs-lookup"><span data-stu-id="c76d4-166">Entries</span></span>  | <span data-ttu-id="c76d4-167">Net Amount</span><span class="sxs-lookup"><span data-stu-id="c76d4-167">Net Amount</span></span> |   <span data-ttu-id="c76d4-168">Always</span><span class="sxs-lookup"><span data-stu-id="c76d4-168">Always</span></span>    |      |


3. <span data-ttu-id="c76d4-169">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c76d4-169">Choose the **OK** button.</span></span>  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="c76d4-170">Assigning the Column Layout to the Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="c76d4-170">Assigning the Column Layout to the Account Schedule Name</span></span>  
<span data-ttu-id="c76d4-171">Ken is now ready to assign the column layout to the account schedule name.</span><span class="sxs-lookup"><span data-stu-id="c76d4-171">Ken is now ready to assign the column layout to the account schedule name.</span></span>  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="c76d4-172">To assign the column layout to the account schedule name</span><span class="sxs-lookup"><span data-stu-id="c76d4-172">To assign the column layout to the account schedule name</span></span>  

1.  <span data-ttu-id="c76d4-173">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="c76d4-173">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span></span>  
2.  <span data-ttu-id="c76d4-174">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span><span class="sxs-lookup"><span data-stu-id="c76d4-174">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span></span>  

### <a name="to-view-and-print-the-cash-flow-forecast"></a><span data-ttu-id="c76d4-175">To view and print the cash flow forecast</span><span class="sxs-lookup"><span data-stu-id="c76d4-175">To view and print the cash flow forecast</span></span>  
1.  <span data-ttu-id="c76d4-176">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="c76d4-176">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span></span>  
2.  <span data-ttu-id="c76d4-177">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span><span class="sxs-lookup"><span data-stu-id="c76d4-177">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span></span> <span data-ttu-id="c76d4-178">In addition, you can view the formula that is used to calculate the amount.</span><span class="sxs-lookup"><span data-stu-id="c76d4-178">In addition, you can view the formula that is used to calculate the amount.</span></span> <span data-ttu-id="c76d4-179">You can also filter the amounts by date and dimension.</span><span class="sxs-lookup"><span data-stu-id="c76d4-179">You can also filter the amounts by date and dimension.</span></span>  
3.  <span data-ttu-id="c76d4-180">Choose the **Print** action to print the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="c76d4-180">Choose the **Print** action to print the cash flow forecast.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c76d4-181">See Also</span><span class="sxs-lookup"><span data-stu-id="c76d4-181">See Also</span></span>  
 [<span data-ttu-id="c76d4-182">How to: Work with Account Schedules</span><span class="sxs-lookup"><span data-stu-id="c76d4-182">How to: Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)   
 [<span data-ttu-id="c76d4-183">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="c76d4-183">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 [<span data-ttu-id="c76d4-184">Working with</span><span class="sxs-lookup"><span data-stu-id="c76d4-184">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
