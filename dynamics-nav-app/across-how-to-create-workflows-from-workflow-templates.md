---
title: How to Create Workflows from Workflow Templates
description: To save time when creating new workflows, you can create workflows from workflow templates.
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
ms.openlocfilehash: 9c3ebc923b2ffd44a1ec37b312ff4b0d785d8c5c
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7260"
---
# <a name="how-to-create-workflows-from-workflow-templates"></a><span data-ttu-id="a7a1c-103">How to: Create Workflows from Workflow Templates</span><span class="sxs-lookup"><span data-stu-id="a7a1c-103">How to: Create Workflows from Workflow Templates</span></span>
<span data-ttu-id="a7a1c-104">To save time when creating new workflows, you can create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-104">To save time when creating new workflows, you can create workflows from workflow templates.</span></span>  

 <span data-ttu-id="a7a1c-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7a1c-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="a7a1c-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span>  

 <span data-ttu-id="a7a1c-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7a1c-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="a7a1c-108">For more information, see [How to: Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a7a1c-108">For more information, see [How to: Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span></span>  

<span data-ttu-id="a7a1c-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="a7a1c-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="a7a1c-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="a7a1c-112">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a7a1c-112">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-create-a-workflow-from-workflow-template"></a><span data-ttu-id="a7a1c-113">To create a workflow from workflow template</span><span class="sxs-lookup"><span data-stu-id="a7a1c-113">To create a workflow from workflow template</span></span>  
1.  <span data-ttu-id="a7a1c-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a7a1c-115">Choose the **Create Workflow from Template** action.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-115">Choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="a7a1c-116">The **Workflow Templates** window opens.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-116">The **Workflow Templates** window opens.</span></span>  
3.  <span data-ttu-id="a7a1c-117">Select a workflow template, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-117">Select a workflow template, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="a7a1c-118">The **Workflow** window opens for a new workflow containing all the information of the selected template.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-118">The **Workflow** window opens for a new workflow containing all the information of the selected template.</span></span> <span data-ttu-id="a7a1c-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span></span>  
4.  <span data-ttu-id="a7a1c-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span><span class="sxs-lookup"><span data-stu-id="a7a1c-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span></span> <span data-ttu-id="a7a1c-121">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a7a1c-121">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a7a1c-122">See Also</span><span class="sxs-lookup"><span data-stu-id="a7a1c-122">See Also</span></span>  
 [<span data-ttu-id="a7a1c-123">How to: Create Workflows</span><span class="sxs-lookup"><span data-stu-id="a7a1c-123">How to: Create Workflows</span></span>](across-how-to-create-workflows.md)   
 [<span data-ttu-id="a7a1c-124">How to: Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="a7a1c-124">How to: Export and Import Workflows</span></span>](across-how-to-export-and-import-workflows.md)   
 [<span data-ttu-id="a7a1c-125">How to: View Archived Workflow Step Instances</span><span class="sxs-lookup"><span data-stu-id="a7a1c-125">How to: View Archived Workflow Step Instances</span></span>](across-how-to-view-archived-workflow-step-instances.md)   
 [<span data-ttu-id="a7a1c-126">How to: Delete Workflows</span><span class="sxs-lookup"><span data-stu-id="a7a1c-126">How to: Delete Workflows</span></span>](across-how-to-delete-workflows.md)   
 [<span data-ttu-id="a7a1c-127">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span><span class="sxs-lookup"><span data-stu-id="a7a1c-127">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [<span data-ttu-id="a7a1c-128">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="a7a1c-128">Setting Up Workflows</span></span>](across-set-up-workflows.md)   
 [<span data-ttu-id="a7a1c-129">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="a7a1c-129">Using Workflows</span></span>](across-use-workflows.md)   
 [<span data-ttu-id="a7a1c-130">Workflow</span><span class="sxs-lookup"><span data-stu-id="a7a1c-130">Workflow</span></span>](across-workflow.md)   
