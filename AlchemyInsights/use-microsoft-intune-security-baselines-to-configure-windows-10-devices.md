---
title: De beveiligingsbasislijnen van Microsoft Intune gebruiken om Windows 10-apparaten te configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693415"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>De beveiligingsbasislijnen van Microsoft Intune gebruiken voor het configureren van Windows 10-apparaten

Intune-beveiligingsbasislijnen helpen gebruikers en apparaten te beschermen. Beveiligingsbasislijnen zijn vooraf geconfigureerde groepen in Windows-instellingen die worden gebruikt voor het toepassen van een bekende groep instellingen en standaardwaarden die worden aanbevolen door de relevante beveiligingsteams. Door een beveiligingsbasislijnprofiel te maken in Intune, maakt u een sjabloon die uit meerdere apparaatconfiguratieprofielen bestaat.

Wanneer u beveiligingsbasislijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten met Windows 10 of nieuwere versies. Zo schakelt de beveiligingsbasislijn van Microsoft Mobile Device Management (MDM) automatisch (1) BitLocker in voor verwisselbare stations, (2) is het wachtwoord vereist voor het ontgrendelen van een apparaat en (3) worden basisverificatie uitgeschakeld. Als een standaardwaarde niet werkt voor uw omgeving, kunt u de basislijn aanpassen om de instellingen toe te passen die u nodig hebt.

Beveiligingsbasislijnen helpen ook bij het tot stand brengen van een end-to-end veilige werkstroom in Microsoft 365. Hier volgen enkele voordelen van deze functionaliteit:
- Een basislijn voor beveiliging bevat de aanbevolen procedures en aanbevelingen voor instellingen die van invloed zijn op de beveiliging. Omdat Intune partners met het Windows-beveiligingsteam basislijnen voor groepsbeleid maakt, zijn deze aanbevelingen gebaseerd op een betrouwbare begeleiding en uitgebreide ervaring.
- Als Intune nieuw voor u is en niet zeker weet waar u moet beginnen, kunt u met behulp van beveiligingsbasislijnen snel een beveiligd profiel maken en implementeren.
- Als u momenteel een groepsbeleid gebruikt, is een migratie naar Intune voor beheerdoeleinden veel gemakkelijker met beveiligingsbasislijnen, omdat deze beveiligingsbasislijnen zijn ingebouwd in Intune en geavanceerde beheermogelijkheden bevatten.

Zie windows-beveiligingsbasislijnen en [Mobile Device Management voor meer informatie.](https://docs.microsoft.com/windows/client-management/mdm/) [](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)