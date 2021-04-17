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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816343"
---
# <a name="create-a-group"></a>Een groep maken

In dit onderwerp wordt het maken van groepen beschreven.

**Machtiging voor het maken van een groep**

Zorg ervoor dat u gemachtigd bent om een nieuwe groep te maken. Globale beheerders kunnen het maken van groepen uitschakelen in de Azure-portal of het Access-panel. Mogelijk hebt u een beheerder nodig om de nieuwe groep voor u te maken of om u de juiste machtigingen te geven.

**Machtigingen voor het maken van groepen beheren**

1. Globale beheerders kunnen machtigingen voor het maken van groepen beheren (om beveiligingsredenen) of Office 365-groepen die zijn gemaakt in de Azure-portal of het Access-panel, door in Alle groepen Algemeen  >  **(Instellingen)** de opties 'Gebruikers kunnen beveiligingsgroepen maken in Azure-portals' of 'Gebruikers kunnen Office 365-groepen maken in Azure-portals'.
2. U kunt het maken van groepen ook beperken om een groep gebruikers te selecteren als u een Azure Active Directory P1 Premium-licentie hebt.

**Welkomstmelding uitschakelen voor nieuwe Office 365-groepsleden**

De welkomstmelding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365-groepen, kan worden uitgeschakeld door **UnifiedGroupWelcomeMessageEnabled** in te stellen op Onwaar in Powershell. Meer informatie over deze instelling [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

