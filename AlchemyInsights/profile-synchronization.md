---
title: Synchronisatie van het profiel
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371979"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer mijn profielwijzigingen synchroniseren met de SharePoint-profiel van toepassing?

SharePoint Online maakt gebruik van de timeropdracht Active Directory importeren (AD importeren) importeren van gebruikers en groepen in de gebruikersprofieltoepassing. 
  
1. AD importeren wordt gesynchroniseerd wijzigingen van toepassing voor het gebruikersprofiel van de opslag van SharePoint Online. Deze wijzigingen worden verwerkt in batches.
    
2. De timeropdracht wordt uitgevoerd totdat de wijzigingen worden gesynchroniseerd.
    
> [!NOTE]
> Duurt de taak wilt uitvoeren, is afhankelijk van het aantal wijzigingen te verwerken. Een groot aantal wijzigingen duurt langer. Service niveau overeenkomst (SLA) geeft aan dat een wijziging van een gebruiker in de SharePoint Online-map worden weergegeven in de toepassing voor gebruikersprofiel in 24 uur. 
  
[Meer informatie over synchronisatie van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

