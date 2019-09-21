---
title: Rapporten van de klassieke SharePoint-auditlogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068018"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Auditlogboeken van SharePoint en OneDrive

**SharePoint en OneDrive moderne uniforme audit logs van compliance**

- [Schakel registratie van Unified audit in/uit](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Er is geen aanvullende configuratie vereist in SharePoint of OneDrive.

- Gebruik controlelogboekregistratie zoeken om te controleren van de activiteit van de bestanden, map (s), gebruiker (s), machtigingen:

    - [Bestands-en pagina-activiteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Mapactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Activiteiten voordelen en toegang aanvragen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Synchronisatieactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Activiteiten voor site beheer](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Zie [het controlelogboek doorzoeken](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.

**Klassieke SharePoint-audit logboeken**

We migreerden SPO legacy auditing naar Unified audit log (UAL). Dit betekent in wezen dat alle SPO verouderde auditverslagen nu worden gevoed via UAL, en de verouderde controle signalen zijn gemigreerd naar UAL.

Belangrijke wijzigingen:

- Trimmen als een mogelijkheid is niet beschikbaar.
- De sectie waarin u specifieke gebeurtenissen voor controle kiest, is niet beschikbaar. Raadpleeg [dit document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.
- De optie ' locatie ' onder **aangepaste rapporten** is niet beschikbaar. 
- "Openen of downloaden van documenten" gebeurtenissen is niet beschikbaar. 

