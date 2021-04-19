---
title: 'AIP: Beleidsregels gedragen zich niet zoals verwacht'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821622"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Beleidsregels gedragen zich niet zoals verwacht

Azure Information Protection: Beleidsregels werken niet zoals verwacht, zie het volgende voor aanbevolen richtlijnen voor verschillende beleidskwesties:

1. Als u problemen hebt met visuele markeringen, raadpleegt u [Wanneer visuele markeringen worden toegepast.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Als u problemen hebt met automatische labeling, raadpleegt u Voorwaarden configureren voor automatische en aanbevolen classificatie voor [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en Waar de typen gevoelige informatie naar [zoeken.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Als u problemen hebt met de native/pfile-beveiliging, raadpleegt u [bestands-API-configuratie.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Controleer of u beleidsregels met een bereik gebruikt die niet correct zijn geconfigureerd: [Het Azure Information Protection-beleid configureren voor specifieke gebruikers met behulp van beleidsregels met een bereik](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Als automatische labeling niet werkt voor Outlook bij het koppelen van een document met label, controleert u of DRMEncryptProperty niet is gedefinieerd zoals hier wordt beschreven: IRM-registerinstellingen voor [beveiliging.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Als u nog steeds problemen ondervindt, verzamelt u Azure Information Protection-clientlogboeken en koppelt u de geëxporteerde logboeken aan dit ticket.

1. Open een Office-document of maak een nieuw e-mailbericht in Outlook.
2. Klik op **Beveiligen/Gevoeligheid** > **Help en feedback**.
3. Klik op **Logboeken exporteren**.
4. Sla de logboeken op naar uw keuze van locatie en voeg deze toe aan deze serviceaanvraag.

Aanvullende informatiebronnen:

- [Een label configureren voor visuele markeringen voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection-documentatie bekijken](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gevoeligheidslabels gebruiken in Microsoft 365-apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

