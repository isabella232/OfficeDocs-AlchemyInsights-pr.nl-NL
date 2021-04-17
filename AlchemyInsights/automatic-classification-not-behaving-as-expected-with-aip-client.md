---
title: Automatische classificatie gaat niet zoals verwacht met de AIP-client
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820893"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatische classificatie gaat niet zoals verwacht met de AIP-client

Automatische classificatie gaat niet zoals verwacht, gebruik de volgende aanbevolen richtlijnen:

1. Als u problemen ondervindt met automatisch labelen, raadpleegt u [Voorwaarden configureren voor automatische en aanbevolen classificatie voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en [Waar wordt naar gezocht door de typen gevoelige informatie](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Controleer of u beleidsregels met een bereik gebruikt die niet correct zijn geconfigureerd: [Het Azure Information Protection-beleid configureren voor specifieke gebruikers met behulp van beleidsregels met een bereik](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Als automatische labeling niet werkt voor Outlook bij het bij koppelen van een gelabeld document, controleert u of `DRMEncryptProperty` niet is gedefinieerd zoals hier wordt beschreven: [IRM-registerinstellingen voor beveiliging](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Als u de [ingebouwde informatietypen](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) voor uw Azure Information Protection-beleid hebt gebruikt, controleert u of uw inhoud overeenkomt met de verwachte indeling.
5. Controleer of het label correct is geconfigureerd voor **Automatische** of **Aanbevolen** labeling. (**Automatische** labeling is beschikbaar voor alle Microsoft 365-apps, terwijl **Aanbevolen** labeling beschikbaar is voor alle Microsoft 365-apps behalve voor Outlook.)
6. U kunt automatische classificatie niet gebruiken voor documenten en e-mailberichten die eerder handmatig zijn gelabeld of die eerder automatisch met een hogere classificatie zijn gelabeld.  Zie voor meer informatie: [Hoe automatische of aanbevolen labels worden toegepast](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Als u nog steeds problemen ondervindt, verzamelt u clientlogboeken van Azure Information Protection en koppelt u de geëxporteerde logboeken aan uw ondersteuningsticket. Azure Information Protection-logboeken exporteren:
    - Open een Office-document of maak een nieuw e-mailbericht in Outlook.
    - Klik op **Beveiligen/Gevoeligheid** > **Help en feedback**.
    - Klik op **Logboeken exporteren**.
    - Sla de logboeken op de door u gekozen locatie op en voeg ze toe aan uw serviceverzoek.

Raadpleeg voor meer informatie:

- [Voorwaarden configureren voor automatische en aanbevolen classificatie voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Handleidingen voor veelvoorkomende scenario's waarin Azure Information Protection wordt gebruikt](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Information Protection-documentatie bekijken](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection-abonnementen en -functies bekijken](https://azure.microsoft.com/pricing/details/information-protection)
- [Vereisten voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Zelfstudie Aan de slag voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection-client downloaden](https://www.microsoft.com/download/details.aspx?id=53018)
