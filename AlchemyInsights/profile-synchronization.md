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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320704"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wanneer worden mijn profielwijzigingen gesynchroniseerd met SharePoint gebruikersprofieltoepassing?

SharePoint Online gebruikt de Active Directory Import timer job (AD Import) om gebruikers en groepen te importeren in de gebruikersprofieltoepassing. 
  
1. Met AD Importeren worden wijzigingen gesynchroniseerd van de SharePoint Online Directory Store naar de gebruikersprofieltoepassing. Deze wijzigingen worden verwerkt in batches.
    
2. De timer wordt uitgevoerd totdat de wijzigingen zijn gesynchroniseerd.
    
**Opmerking:** De tijd die nodig is om de taak uit te voeren, is afhankelijk van het aantal wijzigingen in het proces. Een groot aantal wijzigingen duurt langer. In de SLA (Service Level Agreement) staat dat een wijziging in een gebruiker in de SharePoint Online Directory binnen 24 uur wordt weerspiegeld in de gebruikersprofieltoepassing. 
  
[Meer informatie over gebruikersprofielsynchronisatie in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

