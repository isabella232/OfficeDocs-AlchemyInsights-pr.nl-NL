---
title: Klassieke SharePoint-controlelogboekrapporten
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741960"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- en OneDrive-controlelogboeken

## <a name="sharepoint-classic-audit-logs"></a>Klassieke SharePoint-controlelogboeken

SPO legacy auditing is gemigreerd naar Unified Audit Log (UAL). Alle SPO legacy audit rapporten worden nu aangedreven via UAL, en de legacy audit signalen zijn gemigreerd naar UAL.

Belangrijkste wijzigingen:

* Trimmen is NIET beschikbaar als een mogelijkheid.
* Het kiezen van specifieke gebeurtenissen om te controleren is NIET beschikbaar. Raadpleeg [dit document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met standaard gecontroleerde gebeurtenissen.
* De optie **Locatie** onder **Aangepaste rapporten** is NIET beschikbaar.
* De optie **Gebeurtenissen voor documenten openen of downloaden** is NIET beschikbaar.

[Controle-instellingen voor een siteverzameling configureren](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- en OneDrive Modern Unified Audit-logboeken op naleving

* [Unified Audit Logging in- of uitschakelen](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Er is geen extra configuratie vereist binnen SharePoint of OneDrive.

Gebruik zoeken naar controlelogboekregistratie om de activiteit van het bestand(en), de map(s), de gebruiker(s), de machtigingen te controleren:

* [Bestands- en pagina-activiteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mapactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activiteiten voor het delen en openen van aanvragen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synchronisatieactiviteiten](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activiteiten voor sitebeheer](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Zie [Het controlelogboek doorzoeken](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.
