---
title: Profielsynchronisatie
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801764"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer wordt mijn profiel gewijzigd met de SharePoint-app voor gebruikersprofielen?

In SharePoint Online wordt de timeropdracht Active Directory-import gebruikt om gebruikers en groepen te importeren in de Gebruikersprofieltoepassing. 
  
1. Wijzigingen in de webversie van SharePoint Online worden gesynchroniseerd met de Gebruikersprofieltoepassing. Deze wijzigingen worden in batches verwerkt.
    
2. De timeropdracht wordt uitgevoerd totdat de wijzigingen worden gesynchroniseerd.
    
> [!NOTE]
> Hoe lang het duurt voordat de taak wordt uitgevoerd, is afhankelijk van het aantal wijzigingen in het proces. Een groot aantal wijzigingen duurt langer. De SLA (Service Level Agreement) geeft aan dat een wijziging van een gebruiker in de SharePoint Online-Directory binnen 24 uur wordt doorgevoerd in de Gebruikersprofieltoepassing. 
  
[Meer informatie over het synchroniseren van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

