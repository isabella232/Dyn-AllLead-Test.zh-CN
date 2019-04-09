---
title: Design Details - General Journal Post Line
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 95c78ed48b9e99049daf0f245c159676185a02b7
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7401"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="2516c-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="2516c-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="2516c-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2516c-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="2516c-105">The redesign makes codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="2516c-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="2516c-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="2516c-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="2516c-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="2516c-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="2516c-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="2516c-108">In This Section</span></span>  
[<span data-ttu-id="2516c-109">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="2516c-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="2516c-110">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="2516c-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="2516c-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="2516c-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="2516c-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="2516c-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="2516c-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="2516c-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="2516c-114">See Also</span><span class="sxs-lookup"><span data-stu-id="2516c-114">See Also</span></span>  
[<span data-ttu-id="2516c-115">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="2516c-115">Working with General Journals</span></span>](ui-work-general-journals.md)
