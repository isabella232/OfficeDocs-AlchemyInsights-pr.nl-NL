---
title: DLP heeft mogelijk een aangepast type nodig
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932653"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP heeft mogelijk een aangepast type nodig

**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd. Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen. In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.

Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag. Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden. Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.

**DLP vereist mogelijk een aangepast informatietype**

Met een DLP-beleid (Data Loss Prevention) u gevoelige gegevens in uw organisatie identificeren en beschermen. In sommige scenario's moet u mogelijk uw eigen **aangepaste** gevoelige informatietype maken om de gegevens van uw organisatie te beschermen.

Uw organisatie moet bijvoorbeeld werknemers-id's of andere gegevens identificeren en beveiligen in een specifieke indeling voor uw organisatie. Zie in dat dan de volgende artikelen voor meer informatie.
  
 **Een ingebouwd gevoelig informatietype aanpassen**
  
Als een ingebouwd gevoelig informatietype met slechts een paar aanpassingen aan uw behoeften zou voldoen, u [een ingebouwd gevoelig informatietype aanpassen.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) U bijvoorbeeld zoekwoorden toevoegen of verwijderen of ondersteunend bewijsmateriaal toevoegen of verwijderen, zoals een datum of adres.
  
 **Een aangepast gevoelig informatietype maken**
  
Maar als u een ander type gevoelige informatie helemaal moet identificeren en beschermen, u [een aangepast gevoelig informatietype maken](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in de gebruikersinterface van het Security & Compliance Center.
  
**Een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell**

Als de gebruikersinterface ten slotte niet alle opties biedt die u nodig hebt, u [een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) Door te beginnen met een XML-bestand, u elke beschikbare optie gebruiken.
