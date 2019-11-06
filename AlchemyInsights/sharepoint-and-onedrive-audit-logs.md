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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992613"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Auditlogboeken van SharePoint en OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassieke SharePoint-audit logboeken

SPO verouderde controle is gemigreerd naar Unified audit log (UAL). Alle SPO verouderde auditrapporten worden nu gevoed via UAL en de verouderde controle signalen zijn gemigreerd naar UAL.

Belangrijke wijzigingen:

* Trimmen is niet beschikbaar als een mogelijkheid.
* Het kiezen van specifieke gebeurtenissen om te controleren is niet beschikbaar. Raadpleeg [dit document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.
* De optie **locatie** onder **aangepaste rapporten** is niet beschikbaar.
* De optie **documenten openen of downloaden** is niet beschikbaar.

[Controle-instellingen voor een siteverzameling configureren](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint en OneDrive moderne uniforme audit logs van compliance

* [Schakel registratie van Unified audit in/uit](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Er is geen aanvullende configuratie vereist in SharePoint of OneDrive.

Gebruik controlelogboekregistratie zoeken om te controleren van de activiteit van de bestanden, map (s), gebruiker (s), machtigingen:

* [Bestands-en pagina-activiteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mapactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activiteiten voordelen en toegang aanvragen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synchronisatieactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activiteiten voor site beheer](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Zie [het controlelogboek doorzoeken](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.
