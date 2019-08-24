---
title: Alleen-lezen voor onderhoud wordt weergegeven wanneer u probeert te gebruiken van SharePoint of OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620718"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Alleen-lezen voor onderhoud wordt weergegeven wanneer u probeert te gebruiken van SharePoint of OneDrive

Gebruikers kunnen een bericht **Alleen-lezen voor onderhoud** tijdens het gebruik van SharePoint of OneDrive voor een van de volgende scenario's. 

-   Een geplande of actieve onderhoudsactiviteiten.  Controleer of ze door te gaan met het [Berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter).
-   Een hoge prioriteit actieve service incident dat zich zou kunnen voordoen. Controleren op eventuele aanbevelingen/incidenten door te gaan voor de [Gezondheid van de Service](https://portal.office.com/adminportal/home#/servicehealth).
-   Een kleine automatische retoucheren herstelscenario dat kan gebeuren als gevolg van een onverwachte gebeurtenissen op de servers die voor minder dan 30 minuten of zo mogelijk laatste. 
    
    Er zijn geen Message Center of Health Service post voor deze kleine terugvorderingen, maar moet worden zeer binnenkort weer in de normale.

In enkele gevallen waargenomen we dat een van de drie scenario's hierboven vermeld zijn de oorzaak, en service is hersteld, maar de gebruikers browsercache nog niet is gewist van.

Probeer om de cache van de browser wissen voordat u naar de site navigeren.

1. Selecteer **Instellingen**en selecteer **Privacy en beveiliging**in de browser Microsoft Edge.
2. Selecteer onder het **wissen bladeren**, **kiezen wat u wilt wissen**.
3. Selecteer **Cookies en gegevens opgeslagen websites**en selecteer **wissen**.

>[!Note] 
> Deze stappen kunnen verschillen bij het gebruik van andere browsers zoals Mozilla Firefox of Google Chrome.

>[!Note] 
> Een andere optie zou zijn voor het openen van uw SharePoint-site of OneDrive in een nieuw venster voor InPrivate-navigatie.