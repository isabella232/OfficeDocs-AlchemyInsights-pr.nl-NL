---
title: Werken met iOS VPP-toepassingen regel id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719952"
---
# <a name="working-with-ios-vpp-applications"></a>Werken met iOS VPP-toepassingen

Lees [Hoe u iOS-apps beheert die zijn aangeschaft via een programma voor volumeaankoop met Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) om meer te weten te komen over functies, beperkingen en stappen om gebruik te maken van het Apple Volume Purchase Program en de ondersteuning hiervoor in Microsoft Intune.
  
 **Veelvoorkomende problemen:** "Ik heb een iOS VPP-app toegewezen aan mijn gebruikers, maar de installatie is mislukt."
  
- Dit kan gebeuren als één VPP-token wordt gebruikt voor meerdere providers voor het beheer van mobiele apparaten. VPP-tokens van Apple mogen slechts bij één provider worden gebruikt. Als u een VPP-token met meerdere providers hebt gebruikt, moet u het token opnieuw uploaden naar Intune.

- De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt. Als u een gebruiksrapport voor uw licenties wilt bekijken, gaat u naar de pagina **Licenties voor Apps-apps** **inAfstemmen.** \> Zie dit artikel voor meer informatie over het terugvorderen van licenties die in gebruik [zijn.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
