---
title: Design Details - Item Tracking Availability
description: The **Item Tracking Lines** and **Item Tracking Summary** windows provide dynamic availability information for serial or lot numbers. The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents. This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled.
documentationcenter: ''
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/26/2017
ms.author: sgroespe
ms.openlocfilehash: e1b2bdba114352e58137e12d463335a5c5a9c539
ms.sourcegitcommit: 02827d275e1341d5c9ddb7b314b43b48a9ac96e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2019
ms.locfileid: "7038"
---
# <a name="design-details-item-tracking-availability"></a>Design Details: Item Tracking Availability
The **Item Tracking Lines** and **Item Tracking Summary** windows provide dynamic availability information for serial or lot numbers. The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents. This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled. For more information, see [Design Details: Item Tracking Lines Window](design-details-item-tracking-lines-window.md).  

 When you open the **Item Tracking Lines** window, availability data is retrieved from the **Item Ledger Entry** table and the **Reservation Entry** table, with no date filter. When you choose the **Serial No.** field or the **Lot No.** field, the **Item Tracking Summary** window opens and shows a summary of the item tracking information in the **Reservation Entry** table. The summary contains the following information about each serial or lot number on the item tracking line:  

|Field|Description|  
|---------------------------------|---------------------------------------|  
|**Total Quantity**|The total quantity of the serial or lot number that is currently in inventory.|  
|**Total Requested Quantity**|The total quantity of the serial or lot number that is currently requested in all documents.|  
|**Current Pending Quantity**|The quantity that is entered in the current instance of the **Item Tracking Lines** window but is not yet committed to the database.|  
|**Total Available Quantity**|The quantity of the serial or lot number that is available for the user to request.<br /><br /> This quantity is calculated from other fields in the window as follows:<br /><br /> total quantity – (total requested quantity + current pending quantity).|  

> [!NOTE]  
>  You can also see the information in the preceding table by using the **Select Entries** function in the **Item Tracking Lines** window.  

 To preserve database performance, availability data is only retrieved once from the database when you open the **Item Tracking Lines** window and when you use the **Refresh Availability** function in the window.  

## <a name="calculation-formula"></a>Calculation Formula  
 As described in the preceding table, the availability of a given serial or lot number is calculated as follows.  

 total available quantity = quantity in inventory – (all demands + quantity not yet committed to the database)  

> [!IMPORTANT]  
>  This formula implies that the serial or lot number availability calculation considers only inventory and ignores projected receipts. Accordingly, supply that is not yet posted to inventory does not affect item tracking availability, as opposed to regular item availability where projected receipts are included.  

## <a name="see-also"></a>See Also  
 [Design Details: Item Tracking](design-details-item-tracking.md)
