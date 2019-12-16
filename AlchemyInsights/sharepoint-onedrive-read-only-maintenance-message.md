---
title: Alleen-lezen voor onderhouds bericht bij een poging om SharePoint of OneDrive te gebruiken
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051276"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Alleen-lezen voor onderhouds bericht bij een poging om SharePoint of OneDrive te gebruiken

Gebruikers kunnen een **alleen-lezen voor onderhouds** bericht ontvangen wanneer u probeert te gebruiken van SharePoint of OneDrive voor een van de volgende scenario's. 

-   Een geplande of actieve onderhoudsactiviteit.  Controleer ze door naar het [berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter)te navigeren.
-   Een actief service incident met hoge prioriteit dat kan optreden. Controleer op eventuele adviezen/incidenten door te navigeren naar de [service status](https://portal.office.com/adminportal/home#/servicehealth).
-   Een kleine auto-Healing herstelscenario dat kan gebeuren als gevolg van onverwachte gebeurtenissen op de servers die kunnen duren voor minder dan 30 min of zo. 
    
    Er zijn geen berichtencentrum of service Health Posts voor deze kleine terugvorderingen, maar je moet heel snel terug naar normaal.

Bij zeer weinig gelegenheden hebben we geconstateerd dat een van de drie hierboven genoemde scenario's de oorzaak zijn geweest, en de service is hersteld, maar de gebruikers browser cache is niet gewist.

Probeer de browser cache te wissen voordat u naar de site navigeert.

1. Selecteer in de Microsoft Edge-browser **instellingen**en selecteer vervolgens **Privacy en beveiliging**.
2. Selecteer onder **wissen browsen** **de optie kiezen wat u wilt wissen**.
3. Selecteer **cookies en opgeslagen website gegevens**en selecteer **Wis**.

>[!Note] 
> Deze stappen kunnen afwijken bij het gebruik van andere browsers zoals Mozilla Firefox of Google Chrome.

>[!Note] 
> Een andere optie is om uw SharePoint-site of OneDrive te openen in een nieuw InPrivate-venster.