---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931425"
---
# <a name="conditional-access-with-intune"></a>Voorwaardelijke toegang met Intune

Als u **Voorwaardelijke toegang** met Intune gebruikt, zijn 3 stappen vereist:

- Maak een **nalevingsbeleid** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pin van ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.
- Maak een **beleid voor voorwaardelijke toegang** dat bepaalt welke resources worden beschermd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze bronnen.  [Een](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) apparaat moet bijvoorbeeld compatibel zijn voordat het toegang krijgt tot zakelijke e-mail.
- Zorg ervoor dat zowel **nalevingsbeleid** als **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers. Hiervoor moeten mogelijk specifieke groepen gebruikers in Azure Active Directory worden gemaakt.

**Nuttige links:**

[Overzicht van apparaatnaleving](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Probleemoplossingsbeleid](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Om e-mail (Exchange online) te beschermen tegen toegang door niet-compatibele apparaten, moeten beide documenten worden gevolgd:

1. [E-mailtoegang beschermen tegen apparaten met EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-mailtoegang beveiligen tegen apparaten met behulp van moderne verificatieclients zoals Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)