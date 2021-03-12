---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704781"
---
# <a name="conditional-access-with-intune"></a>Voorwaardelijke toegang met Intune

Voor  **het gebruik van**  voorwaardelijke toegang met Intune zijn drie stappen vereist:

- Maak een  **compliancebeleid** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)om instellingen te definiëren die moeten worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pincode met ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.
- Maak een **beleid voor voorwaardelijke**  toegang dat bepaalt welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan voor toegang tot deze bronnen.  [Een apparaat moet bijvoorbeeld](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  compatibel zijn voordat u zakelijke e-mail kunt openen.
- Zorg ervoor **dat zowel het nalevingsbeleid**  als het beleid  **voor**  voorwaardelijke toegang zijn gericht op de gewenste groepen gebruikers. Hiervoor moet u mogelijk specifieke groepen gebruikers maken in Azure Active Directory.

**Handige koppelingen:**

[Overzicht van apparaat compliance](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problemen met CA oplossen](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Beleid voor probleemoplossing](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Als u e-mail (Exchange Online) wilt beveiligen tegen toegang door niet-compatibele apparaten, moeten beide documenten worden gevolgd:

1. [E-mailtoegang beveiligen tegen apparaten met EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-mailtoegang beveiligen tegen apparaten met moderne verificatie-clients zoals Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)