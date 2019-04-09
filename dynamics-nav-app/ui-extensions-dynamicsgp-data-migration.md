---
title: Migrate Data from Dynamics GP with the Data Migration Extension
description: Use the Dynamics GP Data Migration extension to migrate customers, vendors, inventory items, and accounts from Dynamics GP to Dynamics NAV.
documentationcenter: ''
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.openlocfilehash: 37478d6757e0ce0728949f58f1de40e76a8012a2
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7132"
---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-nav"></a>The Dynamics GP Data Migration Extension for Dynamics NAV
This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)]. If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Migrate Business Data from Other Finance Systems](upload-data.md).

## <a name="exporting-data-from-dynamics-gp"></a>Exporting Data from Dynamics GP
You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export. For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following types of data:

* Account  
* Customer  
* Item  
* Vendor  

The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company. During the process, supporting setup information is created, such as posting groups. Inventory items will be brought into the system with FIFO as the cost valuation method. Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE[d365fin](includes/d365fin_long_md.md)] does not have account segments.

## <a name="see-also"></a>See Also
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  
