---
title: Een groep maken
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929300"
---
# <a name="create-a-group"></a>Een groep maken

In dit onderwerp wordt het maken van groepen beschreven.

**Machtiging voor het maken van een groep**

Zorg ervoor dat u gemachtigd bent om een nieuwe groep te maken. Globale beheerders kunnen het maken van groepen uitschakelen in de Azure-portal of het Access-panel. Mogelijk hebt u een beheerder nodig om de nieuwe groep voor u te maken of om u de juiste machtigingen te geven.

**Machtigingen voor het maken van groepen beheren**

1. Globale beheerders kunnen machtigingen voor het maken van groepen beheren (om beveiligingsgerelateerde redenen) of Office 365 groepen die zijn gemaakt in de Azure-portal of het Access-panel door in Alle groepen Algemeen  >  **(Instellingen)** de opties 'Gebruikers kunnen beveiligingsgroepen maken in Azure-portal Office 365 s' te kiezen.
2. U kunt het maken van groepen ook beperken om een groep gebruikers te selecteren als u een Azure Active Directory P1-Premium hebt.

**Welkomstmelding uitschakelen voor nieuwe Office 365 groepsleden**

De welkomstmelding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365 groepen, kan worden uitgeschakeld door **UnifiedGroupWelcomeMessageEnabled** in te stellen op Onwaar in Powershell. Meer informatie over deze instelling [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

