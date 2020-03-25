---
title: DLP werkt niet zoals verwacht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932617"
---
# <a name="dlp-not-working-as-expected"></a>DLP werkt niet zoals verwacht

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

 **DLP instellen**

Heeft u problemen met **Data Loss Prevention (DLP)** in Office 365 werkt niet zoals verwacht? Zorg er dan voor dat uw **DLP-beleid** correct is ingesteld en dat uw gegevens bevatten waar het **DLP-beleid** naar op zoek is wanneer het wordt geëvalueerd.
  
Met DLP-beleid u gevoelige informatie in uw organisatie identificeren en beveiligen. Als u DLP-beleid wilt instellen, gebruikt u de informatie [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Waar dlp-beleid naar zoekt**
  
Wanneer u de **ingebouwde gevoelige informatietypen** in het Office 365 Security and Compliance Center gebruikt, zoekt het DLP-beleid naar specifieke patronen en elementen bij het detecteren van deze gevoelige typen.
  
- **Ingebouwde gevoelige informatietypen**

    Zie voor informatie over de ingebouwde gevoelige typen en waar een DLP-beleid naar zoekt bij het detecteren van het gevoelige type: [Waar de gevoelige informatietypen naar zoeken.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- **Aangepaste gevoelige informatietypen**

    Als u aangepaste gevoelige informatietypen probeert te maken, gebruikt u het volgende artikel voor informatie over het maken van een aangepast gevoelig type: [Een aangepast gevoelig informatietype maken](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Een DLP-beleid testen**

Als u uw gegevens wilt testen met een ingebouwd of aangepast gevoelig informatietype, gebruikt u de optie **Testtype** onder**Gevoelige infotypen** **classificaties** > . Zie [Aangepaste gevoelige informatietypen testen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)voor meer informatie .

 **Rapporten**
  
- Krijg gevoelige gegevensinzichten met [DLP-rapporten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Zie specifieke details van de gebeurtenis met een [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
