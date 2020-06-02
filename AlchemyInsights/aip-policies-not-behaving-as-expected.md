---
title: 'AIP: Beleid dat zich niet gedraagt zoals verwacht'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493021"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Beleid dat zich niet gedraagt zoals verwacht

Azure Information Protection: Beleid dat zich niet gedraagt zoals verwacht, zie de volgende richtlijnen voor verschillende beleidsproblemen:

1. Als u problemen ondervindt met visuele markeringen, controleert u [Wanneer visuele markeringen worden toegepast.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Als u problemen ondervindt met automatische etikettering, raadpleegt u [Hoe u de voorwaarden voor automatische en aanbevolen classificatie voor Azure Information Protection configureert](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en waar de gevoelige [informatietypen naar zoeken.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
3. Als u problemen ondervindt met native/pfile-beveiliging, raadpleegt u [de configuratie van bestands-API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Controleer of u scoped policies gebruikt die niet goed zijn geconfigureerd: [het azure-beleid voor informatiebescherming configureren voor specifieke gebruikers met behulp van scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Als automatische etikettering niet werkt voor Outlook bij het koppelen van een gelabeld document, controleert u of DRMEncryptProperty niet is gedefinieerd zoals hier beschreven: [IRM-registerinstellingen voor beveiliging](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Als u nog steeds problemen ondervindt, u azure information protection-clientlogboeken verzamelen en de geëxporteerde logboeken aan dit ticket koppelen.

1. Open een Office-document of maak een nieuwe e-mail in Outlook.
2. Klik op Help en feedback **over bescherming/gevoeligheid**  >  **Help and feedback**.
3. Klik **op Logboeken exporteren**.
4. Sla de logboeken op naar keuze van de locatie en voeg ze toe aan deze serviceaanvraag.

Aanvullende informatiebronnen:

- [Een label configureren voor visuele markeringen voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Documentatie over Azure Information Protection controleren](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gevoeligheidslabels gebruiken in Office-apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

