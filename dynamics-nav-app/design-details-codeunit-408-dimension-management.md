---
title: Design Details - Codeunit 408 Dimension Management
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
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
ms.openlocfilehash: 8e147b85d018ffb35871ed38c0ff404bc1f9824b
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7258"
---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="97ecc-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="97ecc-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="97ecc-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="97ecc-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="97ecc-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="97ecc-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="97ecc-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="97ecc-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="97ecc-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="97ecc-107">Modified Functions</span></span>  

|<span data-ttu-id="97ecc-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="97ecc-108">Function Name</span></span>|<span data-ttu-id="97ecc-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="97ecc-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="97ecc-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="97ecc-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="97ecc-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="97ecc-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="97ecc-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="97ecc-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="97ecc-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="97ecc-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="97ecc-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="97ecc-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="97ecc-117">CheckDimValueComb</span></span>|<span data-ttu-id="97ecc-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="97ecc-118">Delete.</span></span> <span data-ttu-id="97ecc-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="97ecc-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="97ecc-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-120">GetDefaultDim</span></span>|<span data-ttu-id="97ecc-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="97ecc-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="97ecc-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="97ecc-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="97ecc-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="97ecc-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="97ecc-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="97ecc-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="97ecc-127">Deleted Functions</span></span>  
 <span data-ttu-id="97ecc-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="97ecc-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="97ecc-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="97ecc-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="97ecc-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="97ecc-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="97ecc-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="97ecc-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="97ecc-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="97ecc-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="97ecc-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-136">InsertDocDim</span></span>  

 <span data-ttu-id="97ecc-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="97ecc-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="97ecc-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="97ecc-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="97ecc-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-141">InsertServContractDim</span></span>  

 <span data-ttu-id="97ecc-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="97ecc-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="97ecc-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="97ecc-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-144">GetDocDim</span></span>  

 <span data-ttu-id="97ecc-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-145">GetProdDocDim</span></span>  

 <span data-ttu-id="97ecc-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="97ecc-146">TypeToTableID1</span></span>  

 <span data-ttu-id="97ecc-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="97ecc-147">TypeToTableID2</span></span>  

 <span data-ttu-id="97ecc-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="97ecc-148">TypeToTableID3</span></span>  

 <span data-ttu-id="97ecc-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="97ecc-149">TypeToTableID4</span></span>  

 <span data-ttu-id="97ecc-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="97ecc-150">TypeToTableID5</span></span>  

 <span data-ttu-id="97ecc-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-152">DeleteDocDim</span></span>  

 <span data-ttu-id="97ecc-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="97ecc-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="97ecc-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="97ecc-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="97ecc-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="97ecc-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-160">ShowDocDim</span></span>  

 <span data-ttu-id="97ecc-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-161">SaveDocDim</span></span>  

 <span data-ttu-id="97ecc-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="97ecc-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="97ecc-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-164">ShowTempDim</span></span>  

 <span data-ttu-id="97ecc-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-165">SaveTempDim</span></span>  

 <span data-ttu-id="97ecc-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="97ecc-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="97ecc-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-168">SaveServContractDim</span></span>  

 <span data-ttu-id="97ecc-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="97ecc-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="97ecc-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="97ecc-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="97ecc-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="97ecc-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="97ecc-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="97ecc-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="97ecc-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="97ecc-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="97ecc-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="97ecc-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="97ecc-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="97ecc-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="97ecc-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="97ecc-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="97ecc-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="97ecc-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="97ecc-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="97ecc-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="97ecc-198">TestDimValue</span></span>  

 <span data-ttu-id="97ecc-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="97ecc-199">TestNewDimValue</span></span>  

 <span data-ttu-id="97ecc-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="97ecc-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="97ecc-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="97ecc-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="97ecc-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-202">GetServContractDim</span></span>  

 <span data-ttu-id="97ecc-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="97ecc-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="97ecc-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="97ecc-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="97ecc-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="97ecc-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="97ecc-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="97ecc-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="97ecc-207">See Also</span><span class="sxs-lookup"><span data-stu-id="97ecc-207">See Also</span></span>
 [<span data-ttu-id="97ecc-208">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="97ecc-208">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
 [<span data-ttu-id="97ecc-209">Design Details: Dimension Set Entries Overview</span><span class="sxs-lookup"><span data-stu-id="97ecc-209">Design Details: Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)   
 [<span data-ttu-id="97ecc-210">Design Details: Searching for Dimension Combinations</span><span class="sxs-lookup"><span data-stu-id="97ecc-210">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)   
 [<span data-ttu-id="97ecc-211">Design Details: Table Structure</span><span class="sxs-lookup"><span data-stu-id="97ecc-211">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
 [<span data-ttu-id="97ecc-212">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="97ecc-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
