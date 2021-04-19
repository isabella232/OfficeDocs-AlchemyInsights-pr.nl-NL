---
title: Het standaard-Yammer-domein wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817950"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Het standaard-/primaire Yammer-domein wijzigen

De Yammer-URL bevat de naam van het huidige primaire domein voor uw Yammer-netwerk. Deze domeinnaam komt mogelijk niet overeen met de naam van het primaire domein dat is ingesteld in Office 365 of Azure AD. Er zijn verschillen in gedrag die zijn gebaseerd op het aantal aangepaste domeinen dat aan de tenant is toegevoegd en of Yammer deel uitmaakt van een ondersteunde configuratie (1 tenant: 1 netwerk ofwel 1:1). Er is documentatie over [Yammer-domeinen en Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) beschikbaar.

De meest voorkomende reden dat u een onjuist domein ziet, is dat er meerdere Yammer-netwerken zijn en dat deze moeten worden geconsolideerd. [Consolideren naar één netwerk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) met behulp van het netwerkmigratieprogramma is een belangrijke eerste stap. Voer deze stap uit voordat u uw primaire domein instelt.

**Geen aangepaste domeinen**

Voor nieuwe tenants wordt voor Yammer het standaarddomein (bijvoorbeeld fabrikam.onmicrosoft.com) van de tenant gebruikt. Het primaire domein is ingesteld op yammer.com/fabrikam.onmicrosoft.com.

**Eén aangepast domein**

Yammer selecteert automatisch het aangepaste domein (bijvoorbeeld fabrikam.com) van de tenant als het primaire domein in Yammer. Het is ingesteld op yammer.com/fabrikam.com. Deze wijziging is aangebracht door de domeinsynchronisatieservice en het kan tot 24 uur duren voordat deze van kracht is.

**Meerdere aangepaste domeinen**

Yammer kan een primair domein hebben dat verschilt van het standaardtenantdomein. Aangezien er meerdere aangepaste domeinen zijn, probeert Yammer niet te raden welk van de beschikbare domeinen juist is. U moet een ondersteuningscase openen om aan te vragen dat de naam van het primaire domein wordt gewijzigd in het primaire domein van uw keuze.

**Aanvullende informatie voor het oplossen van problemen**

In sommige gevallen kunnen domeinen tussen tenants zijn verplaatst en kan de domeinsynchronisatieservice niet worden uitgevoerd. U kunt niet alleen te maken krijgen met een onjuist primair domein maar er kunnen zich ook aanmeldingsproblemen of andere problemen voordoen. Om dit probleem op te lossen, moeten domeinen mogelijk naar het juiste netwerk worden verplaatst met de hulp van Microsoft-ondersteuning. In deze situatie is er direct hulp nodig en kan het enige tijd duren om dit op te lossen, met name als er sprake is van een zeer lange lijst met domeinnamen. Open een ondersteuningscase om hulp te krijgen bij het oplossen van dergelijke problemen.

Wanneer u met een ondersteuningsmedewerker werkt, controleert hij/zij of domeinen worden geverifieerd in een tenant die door u wordt beheerd. Mogelijk worden er aanvullende verificatievragen over uw domeinen gesteld als deze zijn toegevoegd aan uw tenant maar niet door DNS worden geverifieerd. Zorg ervoor dat domeinen door DNS worden geverifieerd om het proces te versnellen.
