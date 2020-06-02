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
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509595"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- en OneDrive-controlelogboeken

## <a name="sharepoint-classic-audit-logs"></a>SharePoint-klassieke controlelogboeken

SPO legacy auditing is gemigreerd naar Unified Audit Log (UAL). Alle SPO legacy audit rapporten worden nu aangedreven via UAL, en de legacy audit signalen zijn gemigreerd naar UAL.

Belangrijkste wijzigingen:

* Trimmen is NIET beschikbaar als mogelijkheid.
* Het kiezen van specifieke gebeurtenissen om te controleren is NIET beschikbaar. Raadpleeg [dit document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.
* De optie **Locatie** onder **Aangepaste rapporten** is NIET beschikbaar.
* De optie **Gebeurtenissen openen of downloaden** is NIET beschikbaar.

[Controle-instellingen configureren voor een siteverzameling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- en OneDrive Modern Unified Audit-logboeken vanuit compliance

* [Unified Audit Logging in-/uitschakelen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Er is geen extra configuratie vereist in SharePoint of OneDrive.

Gebruik zoeken naar controlelogboekregistratie om de activiteit van het bestand(en), map(s), gebruikers(en) te controleren:

* [Bestands- en paginaactiviteiten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mapactiviteiten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activiteiten voor aanvragen delen en openen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synchronisatieactiviteiten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activiteiten voor sitebeheer](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Zie [Zoeken in het controlelogboek](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.
