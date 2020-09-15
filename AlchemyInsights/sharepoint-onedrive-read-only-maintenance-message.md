---
title: Alleen-lezen voor onderhouds bericht bij het gebruik van SharePoint of OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670827"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Alleen-lezen voor onderhouds bericht bij het gebruik van SharePoint of OneDrive

Gebruikers kunnen een **alleen-lezen bericht ontvangen voor onderhoud** wanneer ze probeert SharePoint of OneDrive te gebruiken voor één van de volgende scenario's. 

-   Een geplande of actieve onderhouds activiteit.  Ga naar het [berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter)om dit te controleren.
-   Een hoge prioriteit, een actief service voorval dat mogelijk wordt uitgevoerd. Kijk op een of meer adviseurs/incidenten door naar [service status](https://portal.office.com/adminportal/home#/servicehealth)te navigeren.
-   Een klein herstelscenario met automatisch herstel dat kan optreden vanwege eventuele onverwachte gebeurtenissen op de servers die voor minder dan 30 minuten duren. 
    
    Er zijn geen berichtencentrum of service statusberichten voor deze kleine herdetecties, maar u moet altijd weer normaal zijn.

In slechts een paar gevallen hebben we vastgesteld dat een van de drie scenario's hierboven de oorzaak was en de service hersteld is, maar de browsercache van de gebruikers niet is gewist.

Probeer de cache van de browser te wissen voordat u naar de site navigeert.

1. Selecteer in de browser Microsoft Edge **instellingen**en selecteer vervolgens **Privacy en beveiliging**.
2. Selecteer onder **Browse wissen**de **optie Selecteer wat u wilt wissen**.
3. Selecteer **cookies en opgeslagen websitegegevens**en selecteer **wissen**.

>[!Note] 
> Deze stappen kunnen verschillen wanneer u andere browsers gebruikt, zoals Mozilla Firefox of Google Chrome.

>[!Note] 
> Een andere mogelijkheid is om uw SharePoint-site of OneDrive te openen in een nieuw InPrivate-venster.