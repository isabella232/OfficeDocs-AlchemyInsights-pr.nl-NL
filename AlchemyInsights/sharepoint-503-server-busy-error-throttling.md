---
title: SharePoint Online-beperking
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931221"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online-beperking

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

**503-server is bezet fout**

Gebruikers kunnen een 503-server ontvangen die een fout heeft wanneer ze naar SharePoint- of OneDrive-sites proberen te navigeren. 

Deze fout kan worden veroorzaakt door beperking binnen de SharePoint-service. SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden. Beperking beperkt het aantal gebruikersacties of gelijktijdige aanroepen (per script of code) om overmatig gebruik van resources te voorkomen. 

Zie [Voorkomen dat u wordt beperkt of geblokkeerd in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)voor meer informatie over beperking.

Als u van mening bent dat deze fout niets te maken heeft met beperking, u controleren of er actief onderhoud plaatsvindt op uw tenant door naar het [Berichtencentrum](https://portal.office.com/adminportal/home#/MessageCenter)te navigeren.

 Tot slot, zorg ervoor dat u de [pagina Service gezondheid](https://portal.office.com/adminportal/home#/servicehealth) om te controleren op eventuele adviezen / incidenten die zich kunnen voordoen.

