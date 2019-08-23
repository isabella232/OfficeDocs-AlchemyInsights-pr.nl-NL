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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554328"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer mijn profielwijzigingen synchroniseren met de SharePoint-profiel van toepassing?

SharePoint Online maakt gebruik van de timeropdracht Active Directory importeren (AD importeren) importeren van gebruikers en groepen in de gebruikersprofieltoepassing. 
  
1. AD importeren wordt gesynchroniseerd wijzigingen van toepassing voor het gebruikersprofiel van de opslag van SharePoint Online. Deze wijzigingen worden verwerkt in batches.
    
2. De timeropdracht wordt uitgevoerd totdat de wijzigingen worden gesynchroniseerd.
    
> [!NOTE]
> Duurt de taak wilt uitvoeren, is afhankelijk van het aantal wijzigingen te verwerken. Een groot aantal wijzigingen duurt langer. Service niveau overeenkomst (SLA) geeft aan dat een wijziging van een gebruiker in de SharePoint Online-map worden weergegeven in de toepassing voor gebruikersprofiel in 24 uur. 
  
[Meer informatie over synchronisatie van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

