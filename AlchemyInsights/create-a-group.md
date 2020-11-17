---
title: Een groep maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088687"
---
# <a name="create-a-group"></a>Een groep maken

In dit onderwerp wordt het maken van groepen beschreven.

**Machtiging om een groep te maken**

Zorg ervoor dat u gemachtigd bent om een nieuwe groep te maken. Globale beheerders kunnen het maken van groepen in het Azure-portal of toegangsvenster uitschakelen. U hebt mogelijk een beheerder nodig om de nieuwe groep voor u te maken of om u de juiste machtigingen te geven.

**Machtigingen voor het maken van groepen beheren**

1. Globale beheerders kunnen het maken van machtigingen voor het maken van groepen (voor beveiligingsredenen) of Office 365-groepen die zijn gemaakt in het Azure-portal of het deelvenster toegang beheren, door ' gebruikers kunnen beveiligingsgroepen maken in azure-portals ' of ' gebruikers kunnen Office 365-groepen maken in azure-portal ' in **alle groepen**  >  **Algemeen (instellingen)**.
2. U kunt ook het maken van groepen beperken voor het selecteren van een groep gebruikers als u een Azure Active Directory P1 Premium-licentie hebt.

**Welkom melding uitschakelen voor nieuwe leden van Office 365-groep**

De welkomst melding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365-groepen kan worden uitgeschakeld door **UnifiedGroupWelcomeMessageEnabled** in te stellen op ONWAAR in PowerShell. Meer informatie over deze [instelling.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

