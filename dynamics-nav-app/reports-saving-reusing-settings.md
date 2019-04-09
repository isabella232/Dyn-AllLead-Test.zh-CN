---
title: Apply and Modify Saved Settings on Reports
description: Describes using predefined options and filters to customize a report, and to generate the correct data.
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 09/08/2017
ms.author: jswymer
ms.openlocfilehash: eb06dd6d0a0bc9a168a910eb247dfeed7a144cf4
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "6929"
---
# <a name="managing-saved-settings-on-reports"></a><span data-ttu-id="73298-103">Managing Saved Settings on Reports</span><span class="sxs-lookup"><span data-stu-id="73298-103">Managing Saved Settings on Reports</span></span>
<span data-ttu-id="73298-104">Depending on the report that is run, you might be presented with a page that lets you to set certain options and filters for changing the data that is included in the generated report.</span><span class="sxs-lookup"><span data-stu-id="73298-104">Depending on the report that is run, you might be presented with a page that lets you to set certain options and filters for changing the data that is included in the generated report.</span></span> <span data-ttu-id="73298-105">This page is known as the report request page.</span><span class="sxs-lookup"><span data-stu-id="73298-105">This page is known as the report request page.</span></span> <span data-ttu-id="73298-106">A report can include one or more *saved settings* that you can apply to the report from the request page.</span><span class="sxs-lookup"><span data-stu-id="73298-106">A report can include one or more *saved settings* that you can apply to the report from the request page.</span></span> <span data-ttu-id="73298-107">*Saved settings* are basically predefined options and filters.</span><span class="sxs-lookup"><span data-stu-id="73298-107">*Saved settings* are basically predefined options and filters.</span></span> <span data-ttu-id="73298-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span><span class="sxs-lookup"><span data-stu-id="73298-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span>

<span data-ttu-id="73298-109">You can see the saved settings that are available to you for a report in **Saved Settings** section of the report request page.</span><span class="sxs-lookup"><span data-stu-id="73298-109">You can see the saved settings that are available to you for a report in **Saved Settings** section of the report request page.</span></span>  

## <a name="to-apply-saved-settings-to-a-report"></a><span data-ttu-id="73298-110">To apply saved settings to a report</span><span class="sxs-lookup"><span data-stu-id="73298-110">To apply saved settings to a report</span></span>
1. <span data-ttu-id="73298-111">Open the report.</span><span class="sxs-lookup"><span data-stu-id="73298-111">Open the report.</span></span>

   <span data-ttu-id="73298-112">The report request page appears.</span><span class="sxs-lookup"><span data-stu-id="73298-112">The report request page appears.</span></span>    
2. <span data-ttu-id="73298-113">In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.</span><span class="sxs-lookup"><span data-stu-id="73298-113">In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.</span></span>

   <span data-ttu-id="73298-114">The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries.</span><span class="sxs-lookup"><span data-stu-id="73298-114">The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries.</span></span> <span data-ttu-id="73298-115">The saved settings entry called **Last used options and filters** is always available.</span><span class="sxs-lookup"><span data-stu-id="73298-115">The saved settings entry called **Last used options and filters** is always available.</span></span> <span data-ttu-id="73298-116">These settings are the option and filter values that were used the last time you ran the report.</span><span class="sxs-lookup"><span data-stu-id="73298-116">These settings are the option and filter values that were used the last time you ran the report.</span></span>

## <a name="administer-saved-report-settings-for-users"></a><span data-ttu-id="73298-117">Administer saved report settings for users</span><span class="sxs-lookup"><span data-stu-id="73298-117">Administer saved report settings for users</span></span>
<span data-ttu-id="73298-118">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company.</span><span class="sxs-lookup"><span data-stu-id="73298-118">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company.</span></span> <span data-ttu-id="73298-119">You can assign saved settings for a report to individual users or all users in the company.</span><span class="sxs-lookup"><span data-stu-id="73298-119">You can assign saved settings for a report to individual users or all users in the company.</span></span>

<span data-ttu-id="73298-120">You manage saved settings from page 1506 **Reports Settings**.</span><span class="sxs-lookup"><span data-stu-id="73298-120">You manage saved settings from page 1506 **Reports Settings**.</span></span> <span data-ttu-id="73298-121">To open this page, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Settings**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="73298-121">To open this page, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Settings**, and then choose the related link.</span></span>

<span data-ttu-id="73298-122">From the **Report Settings** page, you can create a new settings from scratch or you can make a copy and modify existing settings.</span><span class="sxs-lookup"><span data-stu-id="73298-122">From the **Report Settings** page, you can create a new settings from scratch or you can make a copy and modify existing settings.</span></span> <span data-ttu-id="73298-123">To modify the options and filters for a settings, choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="73298-123">To modify the options and filters for a settings, choose the **Edit** action.</span></span>

> [!NOTE]
> <span data-ttu-id="73298-124">The saved settings feature on reports is only relevant when the SaveValues property of the request page is set to Yes.</span><span class="sxs-lookup"><span data-stu-id="73298-124">The saved settings feature on reports is only relevant when the SaveValues property of the request page is set to Yes.</span></span> <span data-ttu-id="73298-125">The SaveValues property property is set in the development environment.</span><span class="sxs-lookup"><span data-stu-id="73298-125">The SaveValues property property is set in the development environment.</span></span>  

> [!Important]
> <span data-ttu-id="73298-126">If you create a saved settings item for all users, and it has the same name as an existing saved settings for a specific user, then that user will not be able to use the saved settings that is assigned to everyone.</span><span class="sxs-lookup"><span data-stu-id="73298-126">If you create a saved settings item for all users, and it has the same name as an existing saved settings for a specific user, then that user will not be able to use the saved settings that is assigned to everyone.</span></span>  <span data-ttu-id="73298-127">In the Saved Settings field on the report request page, the user will see two saved settings options with the same name.</span><span class="sxs-lookup"><span data-stu-id="73298-127">In the Saved Settings field on the report request page, the user will see two saved settings options with the same name.</span></span> <span data-ttu-id="73298-128">However, no matter which option he chooses, the user-specific saved settings will be used.</span><span class="sxs-lookup"><span data-stu-id="73298-128">However, no matter which option he chooses, the user-specific saved settings will be used.</span></span>

## <a name="see-also"></a><span data-ttu-id="73298-129">See Also</span><span class="sxs-lookup"><span data-stu-id="73298-129">See Also</span></span>
[<span data-ttu-id="73298-130">Working with Reports</span><span class="sxs-lookup"><span data-stu-id="73298-130">Working with Reports</span></span>](ui-work-report.md)  
