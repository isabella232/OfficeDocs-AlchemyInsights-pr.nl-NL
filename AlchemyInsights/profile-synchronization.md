---
title: Profielsynchronisatie
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768108"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer worden mijn profielwijzigingen gesynchroniseerd met de SharePoint-gebruikersprofieltoepassing?

SharePoint Online gebruikt de timertaak Active Directory Import (AD Import) om gebruikers en groepen te importeren in de gebruikersprofieltoepassing. 
  
1. Ad Import synchroniseert wijzigingen van de SharePoint Online Directory Store naar de gebruikersprofieltoepassing. Deze wijzigingen worden in batches verwerkt.
    
2. De timertaak wordt uitgevoerd totdat de wijzigingen zijn gesynchroniseerd.
    
> [!NOTE]
> De tijd die de taak nodig heeft om uit te voeren, is afhankelijk van het aantal wijzigingen dat moet worden verwerkt. Een groot aantal wijzigingen duurt langer. In de SLA (Service Level Agreement) staat dat een wijziging in de SharePoint Online-map binnen 24 uur wordt weergegeven in de gebruikersprofieltoepassing. 
  
[Meer informatie over synchronisatie van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

