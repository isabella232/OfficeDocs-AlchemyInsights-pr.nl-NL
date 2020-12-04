---
title: Microsoft intune-beveiligings lijnen gebruiken om Windows 10-apparaten te configureren
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573402"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Microsoft intune-beveiligings lijnen gebruiken om Windows 10-apparaten te configureren

InTune-beveiligings basislijns helpen gebruikers en apparaten te beschermen. Met behulp van beveiligings lijnen voor Windows-instellingen worden vooraf geconfigureerde groepen gebruikt om een bekende groep instellingen en standaardwaarden die worden aanbevolen door de relevante beveiligings teams toe te passen. Als u een beveiligings basislijn profiel maakt in intune, maakt u een sjabloon met meerdere apparaatconfiguratie-profielen.

Wanneer u beveiligings basislijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten die worden uitgevoerd op Windows 10 of later. Voorbeeld van MDM-beveiliging (1) wordt BitLocker voor verwisselbare schijven niet automatisch ingeschakeld, (2) het wachtwoord voor het ontgrendelen van een apparaat vereist en (3) basisverificatie uitschakelen. Wanneer een standaardwaarde niet werkt voor uw omgeving, past u de basislijn aan zodat u de gewenste instellingen kunt toepassen.

Met behulp van beveiligings lijnen voor beveiliging kunt u ook een end-to-end beveiligde werkstroom maken in Microsoft 365. Hier volgen enkele voordelen:

- Een beveiligings basislijn bevat de aanbevolen procedures en aanbevelingen voorinstellingen die van invloed zijn op de beveiliging. Aangezien intune-partners met het Windows-beveiligingsteam basislijnen voor groepsbeleidsregels maken, zijn deze aanbevelingen gebaseerd op een ononderbroken richtlijn en een uitgebreide ervaring.
- Als u niet bekend bent met intune en u niet zeker weet waar u moet beginnen, kunt u met behulp van beveiligings lijnen snel een veilig profiel maken en implementeren.
- Als u momenteel een Groepsbeleid gebruikt, wordt de migratie naar intune voor beheerdoeleinden veel eenvoudiger gemaakt met behulp van beveiligings lijnen, omdat ze zijn ingebouwd in intune en de functies voor het beheren van de gesneden Edge bevatten.

Zie [Windows-beveiligings lijnen](https://go.microsoft.com/fwlink/?linkid=2141503) en [beheer van mobiele apparaten](https://go.microsoft.com/fwlink/?linkid=2141701)voor meer informatie.