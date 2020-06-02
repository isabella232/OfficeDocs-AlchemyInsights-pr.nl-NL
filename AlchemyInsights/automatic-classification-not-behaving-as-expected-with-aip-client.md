---
title: Automatische classificatie die zich niet gedraagt zoals verwacht met de AIP-client
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508371"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatische classificatie die zich niet gedraagt zoals verwacht met de AIP-client

Automatische classificatie die zich niet gedraagt zoals verwacht, gebruikt de volgende aanbevolen richtlijnen:

1. Zie [Voorwaarden configureren voor automatische en aanbevolen classificatie voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en wat de gevoelige [informatietypen zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)als u problemen ondervindt met automatische etikettering.
2. Controleer of u scoped policies gebruikt die niet goed zijn geconfigureerd: [het azure-beleid voor informatiebescherming configureren voor specifieke gebruikers met behulp van scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Als automatische etikettering niet werkt voor Outlook bij het koppelen van een gelabeld document, controleert u of `DRMEncryptProperty` dit niet is gedefinieerd als hier beschreven: [IRM-registerinstellingen voor beveiliging](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Als u de [ingebouwde informatietypen](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) hebt gebruikt voor uw Azure Information Protection-beleid, controleert u of uw inhoud overeenkomt met de verwachte indeling.
5. Controleer of het label op de juiste manier is geconfigureerd voor **Automatisch** of **Aanbevolen**. **(Automatische** etikettering is beschikbaar voor alle Office-apps, terwijl **Aanbevolen** beschikbaar is voor alle Office-apps, behalve outlook.)
6. U geen automatische classificatie gebruiken voor documenten en e-mails die eerder handmatig zijn gelabeld of eerder automatisch zijn gelabeld met een hogere classificatie.  Zie voor meer informatie [hoe automatische of aanbevolen labels worden toegepast.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Als u nog steeds problemen ondervindt, u azure information protection-clientlogboeken verzamelen en de geëxporteerde logboeken aan uw ondersteuningsticket koppelen. Azure Information Protection-logboeken exporteren:
    - Open een Office-document of maak een nieuwe e-mail in Outlook.
    - Klik op Help en feedback **over bescherming/gevoeligheid**  >  **Help and feedback**.
    - Klik **op Logboeken exporteren**.
    - Sla de logboeken op naar keuze van de locatie en voeg ze toe aan uw serviceaanvraag.

Zie voor meer informatie:

- [Voorwaarden configureren voor automatische en aanbevolen classificatie voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Handleidingen voor veelvoorkomende scenario's die Azure Information Protection gebruiken](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Documentatie over Azure Information Protection controleren](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Abonnementen en functies voor Azure Information Protection controleren](https://azure.microsoft.com/pricing/details/information-protection)
- [Vereisten voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Zelfstudie snel starten voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection-client downloaden](https://www.microsoft.com/download/details.aspx?id=53018)
