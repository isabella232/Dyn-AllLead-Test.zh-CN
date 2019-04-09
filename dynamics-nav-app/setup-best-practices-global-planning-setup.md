---
title: Best practices for global planning setup
description: The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/08/2017
ms.author: sgroespe
ms.openlocfilehash: 317501a6d35e81971e6b4abce071b62ee9362001
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7331"
---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="0f0c8-103">Setup Best Practices: Global Planning Setup</span><span class="sxs-lookup"><span data-stu-id="0f0c8-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="0f0c8-104">The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-104">The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="0f0c8-105">The following table provides best practices on how to set up selected global planning parameter fields.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="0f0c8-106">For more information about a field, choose the link in the **Setup field** column.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="0f0c8-107">Setup field</span><span class="sxs-lookup"><span data-stu-id="0f0c8-107">Setup field</span></span>|<span data-ttu-id="0f0c8-108">Best practice</span><span class="sxs-lookup"><span data-stu-id="0f0c8-108">Best practice</span></span>|<span data-ttu-id="0f0c8-109">Comment</span><span class="sxs-lookup"><span data-stu-id="0f0c8-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="0f0c8-110">Use Forecast on Locations</span><span class="sxs-lookup"><span data-stu-id="0f0c8-110">Use Forecast on Locations</span></span>|<span data-ttu-id="0f0c8-111">Select if you have forecasts for specific locations.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="0f0c8-112">Components at Location</span><span class="sxs-lookup"><span data-stu-id="0f0c8-112">Components at Location</span></span>|<span data-ttu-id="0f0c8-113">If items are not defined as SKUs, select the location code of your main warehouse.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="0f0c8-114">This also applies if you only use the requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="0f0c8-115">Blank Overflow Level</span><span class="sxs-lookup"><span data-stu-id="0f0c8-115">Blank Overflow Level</span></span>|<span data-ttu-id="0f0c8-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="0f0c8-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="0f0c8-118">Default Dampener Period</span><span class="sxs-lookup"><span data-stu-id="0f0c8-118">Default Dampener Period</span></span>|<span data-ttu-id="0f0c8-119">Set between 1D and 5D.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="0f0c8-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span></span>|<span data-ttu-id="0f0c8-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="0f0c8-122">Default Dampener Quantity</span><span class="sxs-lookup"><span data-stu-id="0f0c8-122">Default Dampener Quantity</span></span>|<span data-ttu-id="0f0c8-123">Set between 5 and 20 percent of the item’s lot size.</span><span class="sxs-lookup"><span data-stu-id="0f0c8-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="0f0c8-124">See Also</span><span class="sxs-lookup"><span data-stu-id="0f0c8-124">See Also</span></span>  
 [<span data-ttu-id="0f0c8-125">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="0f0c8-125">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)   
 [<span data-ttu-id="0f0c8-126">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="0f0c8-126">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)   
 [<span data-ttu-id="0f0c8-127">Set Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="0f0c8-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 [<span data-ttu-id="0f0c8-128">Working with</span><span class="sxs-lookup"><span data-stu-id="0f0c8-128">Working with</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
