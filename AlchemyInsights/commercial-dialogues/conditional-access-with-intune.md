---
title: Voorwaardelijke toegang gebruiken met Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744541"
---
# <a name="using-conditional-access-with-intune"></a>Voorwaardelijke toegang gebruiken met Intune

Voor het gebruik van Voorwaardelijke toegang met Intune zijn drie stappen vereist:

- [Maak een compliancebeleid om instellingen te definiëren die moeten worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pincode van ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Maak een beleid voor voorwaardelijke toegang dat definieert welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze resources. Een apparaat moet bijvoorbeeld compatibel zijn voordat u zakelijke e-mail kunt openen.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zorg ervoor dat zowel compliancebeleid als beleid voor voorwaardelijke toegang zijn gericht op de gewenste groepen gebruikers. Hiervoor zijn mogelijk specifieke groepen gebruikers in Azure Active Directory vereist.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Meer informatie...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
