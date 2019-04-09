---
title: Track User Activity in a Change Log
Description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
documentationcenter: ''
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.openlocfilehash: 1f9be8b3daa5d773455085601578b04a5d201fc9
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7304"
---
# <a name="logging-changes-in-dynamics-nav"></a><span data-ttu-id="3077c-103">Logging Changes in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="3077c-103">Logging Changes in Dynamics NAV</span></span>
<span data-ttu-id="3077c-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span><span class="sxs-lookup"><span data-stu-id="3077c-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="3077c-105">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span><span class="sxs-lookup"><span data-stu-id="3077c-105">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="3077c-106">The change log collects all changes that are made to the table.</span><span class="sxs-lookup"><span data-stu-id="3077c-106">The change log collects all changes that are made to the table.</span></span>  

## <a name="working-with-the-change-log"></a><span data-ttu-id="3077c-107">Working with the Change log</span><span class="sxs-lookup"><span data-stu-id="3077c-107">Working with the Change log</span></span>
<span data-ttu-id="3077c-108">A common problem in many financial systems is to locate the origin of errors and changes in data.</span><span class="sxs-lookup"><span data-stu-id="3077c-108">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="3077c-109">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="3077c-109">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="3077c-110">The change log lets you track all direct modifications a user makes to data in the database.</span><span class="sxs-lookup"><span data-stu-id="3077c-110">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="3077c-111">You must specify each table and field that you want the system to log, and then you must activate the change log.</span><span class="sxs-lookup"><span data-stu-id="3077c-111">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="3077c-112">You activate and deactivate the change log in the **Change Log Setup** window.</span><span class="sxs-lookup"><span data-stu-id="3077c-112">You activate and deactivate the change log in the **Change Log Setup** window.</span></span> <span data-ttu-id="3077c-113">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span><span class="sxs-lookup"><span data-stu-id="3077c-113">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span> <span data-ttu-id="3077c-114">This cannot be turned off.</span><span class="sxs-lookup"><span data-stu-id="3077c-114">This cannot be turned off.</span></span>  

<span data-ttu-id="3077c-115">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span><span class="sxs-lookup"><span data-stu-id="3077c-115">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="3077c-116">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span><span class="sxs-lookup"><span data-stu-id="3077c-116">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span></span> <span data-ttu-id="3077c-117">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span><span class="sxs-lookup"><span data-stu-id="3077c-117">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3077c-118">See Also</span><span class="sxs-lookup"><span data-stu-id="3077c-118">See Also</span></span>
[<span data-ttu-id="3077c-119">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="3077c-119">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="3077c-120">Sorting</span><span class="sxs-lookup"><span data-stu-id="3077c-120">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="3077c-121">Using Search for Page or Report</span><span class="sxs-lookup"><span data-stu-id="3077c-121">Using Search for Page or Report</span></span>](ui-search.md)  
[<span data-ttu-id="3077c-122">How to: Manage Users and Permissions</span><span class="sxs-lookup"><span data-stu-id="3077c-122">How to: Manage Users and Permissions</span></span>](ui-how-users-permissions.md)    
[<span data-ttu-id="3077c-123">Working with</span><span class="sxs-lookup"><span data-stu-id="3077c-123">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
