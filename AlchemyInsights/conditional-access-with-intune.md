---
title: Voorwaardelijke toegang met intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807654"
---
# <a name="conditional-access-with-intune"></a>Voorwaardelijke toegang met intune

Voor  **voorwaardelijke toegang**  met intune zijn drie stappen nodig:

- Maak een  **nalevingsbeleid**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) om te bepalen welke instellingen moeten voldoen voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pincode van minimaal 6 cijfers hebben voordat deze als compatibel wordt beschouwd.
- Maak een **voorwaardelijk toegangsbeleid**  om te bepalen welke bronnen worden beveiligd, en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot de bronnen.  Een apparaat moet [bijvoorbeeld](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) voldoen voordat u zakelijke e-mail opent.
- Zorg ervoor dat zowel **nalevingsbeleid**  als  **beleid voor voorwaardelijke toegang**  is bedoeld voor de gewenste groepen gebruikers. Daarom moet u mogelijk specifieke groepen gebruikers maken in azure Active Directory.

**Handige koppelingen:**

[Overzicht van apparaatcompatibiliteit](https://docs.microsoft.com/intune/device-compliance-get-started)

[Oplossing van een certificeringsinstantie](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Beleid voor probleemoplossing](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Als u E-mail (Exchange Online) van Access wilt beschermen tegen niet-compatibele apparaten, moet u beide documenten volgen:

1. [E-mail toegang beschermen tegen apparaten met EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-mail toegang beschermen tegen apparaten met moderne verificatie-clients, zoals Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)