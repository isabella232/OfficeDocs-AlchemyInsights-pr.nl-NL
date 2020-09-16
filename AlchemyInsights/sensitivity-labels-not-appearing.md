---
title: Tekstlabels voor vertrouwelijkheid niet weergegeven
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801179"
---
# <a name="sensitivity-labels-not-appearing"></a>Tekstlabels voor vertrouwelijkheid niet weergegeven

Met gevoelige labels kunt u uw vertrouwelijke inhoud classificeren en beschermen. U kunt ze maken in het nalevings centrum van Microsoft 365, Microsoft 365 Beveiligingscentrum of Microsoft 365 Security & compliance, onder classificatie > voor gevoeligheid-labels. Zie voor meer informatie over deze functie: [overzicht van palletlabels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Controleer het volgende als u uw gevoeligheids labels hebt geconfigureerd, maar deze niet in de Microsoft 365-apps worden weergegeven:

- Ga na of het vertrouwelijkheids label is [gepubliceerd](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) naar de gewenste gebruikers en groepen.

- Ga na of de gebruiker een app gebruikt die de vertrouwelijkheids labels ondersteunt-Zie [de palletlabels in uw document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Als u [Azure Information Protection-labels migreert](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), moet u rekening houden met de [onderstaande overwegingen.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Ondersteuning voor preventie van gegevensverlies (DLP): momenteel kunnen alleen Bewaar labels als voorwaarde worden gebruikt in DLP-beleid.  Ondersteuning voor vertrouwelijkheids labels in een DLP-beleid is nog niet beschikbaar maar we werken eraan.

- Wanneer versleuteling op een gevoeligheids label is ingeschakeld, kunt u kiezen voor:
    - Nu machtigingen toewijzen
    - Gebruikersmachtigingen laten toewijzen


Zie [bekende problemen met gevoeligheid-labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)voor meer informatie over mogelijke problemen.