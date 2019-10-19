---
title: Profielsynchronisatie
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554328"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer verandert mijn profielsynchronisatie met de SharePoint-Gebruikersprofieltoepassing?

SharePoint Online gebruikt de timeropdracht voor het importeren van Active Directory (AD import) om gebruikers en groepen te importeren in de Gebruikersprofieltoepassing. 
  
1. AD import synchroniseert wijzigingen van het SharePoint Online-adreslijstarchief naar de Gebruikersprofieltoepassing. Deze wijzigingen worden verwerkt in batches.
    
2. De timeropdracht wordt uitgevoerd totdat de wijzigingen zijn gesynchroniseerd.
    
> [!NOTE]
> De tijd die het duurt voordat de taak wordt uitgevoerd, is afhankelijk van het aantal wijzigingen dat moet worden verwerkt. Een groot aantal wijzigingen duurt langer. De Service Level Agreement (SLA) staat dat een wijziging aan een gebruiker in de SharePoint Online-map wordt weergegeven in de toepassing gebruikersprofiel in 24 uur. 
  
[Meer informatie over synchronisatie van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

