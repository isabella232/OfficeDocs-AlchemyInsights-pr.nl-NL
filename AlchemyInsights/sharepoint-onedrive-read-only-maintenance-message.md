---
title: Read-Only voor onderhoudsbericht bij het gebruik van SharePoint of OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910541"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only voor onderhoudsbericht bij het gebruik van SharePoint of OneDrive

Gebruikers ontvangen mogelijk een **bericht alleen-lezen** voor onderhoud wanneer ze een SharePoint of OneDrive gebruiken voor een van de volgende scenario's. 

-   Een geplande of actieve onderhoudsactiviteit.  Controleer of ze zijn door naar het Berichtencentrum [te navigeren.](https://portal.office.com/adminportal/home#/messagecenter)
-   Een incident met een hoge prioriteit, actieve service die mogelijk plaatsvindt. Controleer op eventuele adviezen/incidenten door naar Service health [te gaan.](https://portal.office.com/adminportal/home#/servicehealth)
-   Een secundair scenario voor automatisch herstel dat kan plaatsvinden als gevolg van onverwachte gebeurtenissen op de servers die minder dan 30 minuten of zo kunnen duren. 
    
    Er zijn geen Berichtencentrum of Service health-berichten voor deze secundaire herstelberichten, maar u moet binnenkort weer normaal zijn.

In zeer weinig gevallen hebben we vastgesteld dat een van de drie bovenstaande scenario's de oorzaak is en dat de service is hersteld, maar dat de browsercache van gebruikers niet is geweken.

Probeer de browsercache te wissen voordat u naar de site gaat.

1. Selecteer in Microsoft Edge browser **Instellingen** en selecteer **vervolgens Privacy en beveiliging.**
2. Selecteer **onder Bladeren verwijderen** de optie Kiezen wat u wilt **verwijderen.**
3. Selecteer **Cookies en opgeslagen websitegegevens** en selecteer **Verwijderen.**

>[!Note] 
> Deze stappen kunnen verschillen wanneer u andere browsers gebruikt, zoals Mozilla Firefox of Google Chrome.

>[!Note] 
> Een andere optie is het openen van uw SharePoint of OneDrive in een nieuw InPrivate-venster.