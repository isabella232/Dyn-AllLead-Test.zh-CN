---
title: Managing Personalization as an Administrator
description: Learn how to customize the user interface to suit your way of working.
documentationcenter: ''
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.openlocfilehash: c178267c72476fe59a64aaf894c3c8d4c824a7ce
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7005"
---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="27685-103">Managing Personalization as an Administrator</span><span class="sxs-lookup"><span data-stu-id="27685-103">Managing Personalization as an Administrator</span></span>
<span data-ttu-id="27685-104">Users can personalize their workspace to suit their own preferences.</span><span class="sxs-lookup"><span data-stu-id="27685-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="27685-105">As an administrator, you can control and manage personalization by:</span><span class="sxs-lookup"><span data-stu-id="27685-105">As an administrator, you can control and manage personalization by:</span></span>

-   <span data-ttu-id="27685-106">Enabling or disabling the personalization feature for the entire the application ([!INCLUDE[nav_web_md](includes/nav_web_md.md)] only).</span><span class="sxs-lookup"><span data-stu-id="27685-106">Enabling or disabling the personalization feature for the entire the application ([!INCLUDE[nav_web_md](includes/nav_web_md.md)] only).</span></span> <span data-ttu-id="27685-107">You cannot disable personalization on a global basis for the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)].</span><span class="sxs-lookup"><span data-stu-id="27685-107">You cannot disable personalization on a global basis for the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)].</span></span>
-   <span data-ttu-id="27685-108">Enabling or disabling the personalization feature for users of a specific profile.</span><span class="sxs-lookup"><span data-stu-id="27685-108">Enabling or disabling the personalization feature for users of a specific profile.</span></span>
-   <span data-ttu-id="27685-109">Clearing any page personalizations that users have made.</span><span class="sxs-lookup"><span data-stu-id="27685-109">Clearing any page personalizations that users have made.</span></span>

## <a name="EnablePersonalization"></a><span data-ttu-id="27685-110">Enabling or Disabling Personalization in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)]</span><span class="sxs-lookup"><span data-stu-id="27685-110">Enabling or Disabling Personalization in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)]</span></span> 
<span data-ttu-id="27685-111">By default, personalization is not enabled in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)].</span><span class="sxs-lookup"><span data-stu-id="27685-111">By default, personalization is not enabled in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)].</span></span> <span data-ttu-id="27685-112">To enable personalization, you modify the configuration file (navsettings.json) of the [!INCLUDE[nav_web_server_instance_md](includes/nav_web_server_instance_md.md)] instance for the Web client to include this line:</span><span class="sxs-lookup"><span data-stu-id="27685-112">To enable personalization, you modify the configuration file (navsettings.json) of the [!INCLUDE[nav_web_server_instance_md](includes/nav_web_server_instance_md.md)] instance for the Web client to include this line:</span></span>

```
"PersonalizationEnabled": "True"
```

<span data-ttu-id="27685-113">If you want to disable personalization in the Web client, remove this line.</span><span class="sxs-lookup"><span data-stu-id="27685-113">If you want to disable personalization in the Web client, remove this line.</span></span>

<span data-ttu-id="27685-114">For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics-nav/configuring-microsoft-dynamics-nav-web-client-by-modifying-the-web.config-file#WebClientSettingsFile).</span><span class="sxs-lookup"><span data-stu-id="27685-114">For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics-nav/configuring-microsoft-dynamics-nav-web-client-by-modifying-the-web.config-file#WebClientSettingsFile).</span></span>

## <a name="disabling-personalization-for-a-profile"></a><span data-ttu-id="27685-115">Disabling Personalization for a Profile</span><span class="sxs-lookup"><span data-stu-id="27685-115">Disabling Personalization for a Profile</span></span>
<span data-ttu-id="27685-116">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span><span class="sxs-lookup"><span data-stu-id="27685-116">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>
1.  <span data-ttu-id="27685-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="27685-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>
2.  <span data-ttu-id="27685-118">Select the profile in the list that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="27685-118">Select the profile in the list that you want to modify.</span></span>
3.  <span data-ttu-id="27685-119">Select the **Disable personalization** check box, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="27685-119">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

## <a name="clearing-user-personalizations"></a><span data-ttu-id="27685-120">Clearing User Personalizations</span><span class="sxs-lookup"><span data-stu-id="27685-120">Clearing User Personalizations</span></span>
<span data-ttu-id="27685-121">Clearing page personalization changes the page back to its original layout before any personalization was made.</span><span class="sxs-lookup"><span data-stu-id="27685-121">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="27685-122">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span><span class="sxs-lookup"><span data-stu-id="27685-122">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="27685-123">To clear user personalizations by using the Delete User Personalization page</span><span class="sxs-lookup"><span data-stu-id="27685-123">To clear user personalizations by using the Delete User Personalization page</span></span>
<span data-ttu-id="27685-124">The **Delete User Personalization** page enables you to clear personalization on a per-page, per-user basis.</span><span class="sxs-lookup"><span data-stu-id="27685-124">The **Delete User Personalization** page enables you to clear personalization on a per-page, per-user basis.</span></span>

1.  <span data-ttu-id="27685-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="27685-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="27685-126">The page lists all the pages that have been personalized and the user it belongs to.</span><span class="sxs-lookup"><span data-stu-id="27685-126">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="27685-127">A check mark in the **Legacy Personalization** column indicates that the personalization has been done strictly by using [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and/or it has been done in [!INCLUDE[nav_web_md](includes/nav_web_md.md)] prior to [!INCLUDE[navnow_md](includes/navnow_md.md)].</span><span class="sxs-lookup"><span data-stu-id="27685-127">A check mark in the **Legacy Personalization** column indicates that the personalization has been done strictly by using [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and/or it has been done in [!INCLUDE[nav_web_md](includes/nav_web_md.md)] prior to [!INCLUDE[navnow_md](includes/navnow_md.md)].</span></span> <span data-ttu-id="27685-128">Users who try to personalize these pages by using the [!INCLUDE[nav_web_md](includes/nav_web_md.md)] are locked from doing so unless they choose to unlock the page.</span><span class="sxs-lookup"><span data-stu-id="27685-128">Users who try to personalize these pages by using the [!INCLUDE[nav_web_md](includes/nav_web_md.md)] are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="27685-129">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).For more information about personalization between the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and [!INCLUDE[nav_web_md](includes/nav_web_md.md)], see [Working with personalization between the Dynamics NAV Windows and Web client](ui-personalization-overview.md#PersonalizationWinWeb).</span><span class="sxs-lookup"><span data-stu-id="27685-129">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).For more information about personalization between the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and [!INCLUDE[nav_web_md](includes/nav_web_md.md)], see [Working with personalization between the Dynamics NAV Windows and Web client](ui-personalization-overview.md#PersonalizationWinWeb).</span></span>

2. <span data-ttu-id="27685-130">Select the entry that you want to delete, and then choose the **Delete** action.</span><span class="sxs-lookup"><span data-stu-id="27685-130">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="27685-131">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="27685-131">The user will see the changes the next time they sign-in.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="27685-132">To clear user personalizations by using the User Personalization Card page</span><span class="sxs-lookup"><span data-stu-id="27685-132">To clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="27685-133">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span><span class="sxs-lookup"><span data-stu-id="27685-133">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="27685-134">This requires write permission to Table 2000000072 **Profile**.</span><span class="sxs-lookup"><span data-stu-id="27685-134">This requires write permission to Table 2000000072 **Profile**.</span></span>

1.  <span data-ttu-id="27685-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="27685-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="27685-136">The **User Personalization** page lists all users who potentially have personalized pages.</span><span class="sxs-lookup"><span data-stu-id="27685-136">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="27685-137">If you cannot find a user in the list, this means that they do not have any personalized pages.</span><span class="sxs-lookup"><span data-stu-id="27685-137">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="27685-138">Select the user from the list, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="27685-138">Select the user from the list, and then choose the **Edit** action.</span></span>

3.  <span data-ttu-id="27685-139">On the **Actions** tab, choose **Clear Personalized Pages**.</span><span class="sxs-lookup"><span data-stu-id="27685-139">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="27685-140">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="27685-140">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="27685-141">See Also</span><span class="sxs-lookup"><span data-stu-id="27685-141">See Also</span></span>
[<span data-ttu-id="27685-142">Personalization Overview</span><span class="sxs-lookup"><span data-stu-id="27685-142">Personalization Overview</span></span>](ui-personalization-overview.md)  
[<span data-ttu-id="27685-143">Personalizing Your Workspace</span><span class="sxs-lookup"><span data-stu-id="27685-143">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
[<span data-ttu-id="27685-144">Working with</span><span class="sxs-lookup"><span data-stu-id="27685-144">Working with</span></span> [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[<span data-ttu-id="27685-145">How to: Change the Role Center</span><span class="sxs-lookup"><span data-stu-id="27685-145">How to: Change the Role Center</span></span>](change-role.md)  
