---
title: Gebruik Microsoft Intune beveiligingslijnlijnen om de Windows 10 configureren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331980"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Gebruik Microsoft Intune beveiligingslijnlijnen om de Windows 10 configureren

Intune-beveiligingslijnlijnen helpen gebruikers en apparaten te beveiligen. Beveiligingslijnlijnen zijn Windows vooraf geconfigureerde groepen die worden gebruikt om een bekende groep instellingen en standaardwaarden toe te passen die worden aanbevolen door de relevante beveiligingsteams. Door een beveiligingslijnprofiel te maken in Intune, maakt u een sjabloon die bestaat uit meerdere apparaatconfiguratieprofielen.

Wanneer u beveiligingslijnlijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten die op Windows 10 of hoger worden uitgevoerd. Met de MDM-beveiligingslijn (Microsoft Mobile Device Management) wordt BitLocker bijvoorbeeld automatisch inschakelen voor verwisselbare stations, is het wachtwoord vereist voor het ontgrendelen van een apparaat en wordt basisverificatie uitgeschakeld. Wanneer een standaardwaarde niet werkt voor uw omgeving, kunt u de basislijn aanpassen om de instellingen toe te passen die u nodig hebt.

Beveiligingslijnlijnen helpen ook bij het instellen van een end-to-end beveiligde werkstroom in Microsoft 365. Een beveiligingslijn bevat de aanbevolen procedures en aanbevelingen voor instellingen die van invloed zijn op de beveiliging. Intune werkt samen met het Windows beveiligingsteam dat basislijnen maakt voor groepsbeleid, dus deze aanbevelingen zijn gebaseerd op solide richtlijnen en uitgebreide ervaring.

Als u in Intune nieuw bent en niet zeker weet waar u moet beginnen, kunt u met beveiligingslijnlijnen snel een beveiligd profiel maken en implementeren. Als u momenteel een groepsbeleid gebruikt, is het migreren naar Intune voor beheerdoeleinden veel eenvoudiger met beveiligingslijnlijnen, omdat deze zijn ingebouwd in Intune en geavanceerde beheermogelijkheden bevatten.

Zie voor meer informatie [Windows beveiligingslijnlijnen](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) en [Mobiel apparaatbeheer.](https://docs.microsoft.com/windows/client-management/mdm/)

