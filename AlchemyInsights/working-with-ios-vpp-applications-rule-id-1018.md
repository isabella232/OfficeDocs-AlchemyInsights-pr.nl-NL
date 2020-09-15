---
title: Werken met regels voor VPP VPP-toepassingen 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688941"
---
# <a name="working-with-ios-vpp-applications"></a>Werken met VPP-toepassingen van iOS

Meer informatie over het [beheren van Ios-apps die u hebt gekocht via een volume aankoopprogramma met Microsoft intune](https://docs.microsoft.com/intune/vpp-apps-ios) voor informatie over functies, beperkingen en stappen voor het gebruik van het Apple volume Purchase Program en de ondersteuning hiervan in Microsoft intune.
  
 **Veelvoorkomende problemen:** ' Ik heb een iOS VPP-app aan mijn gebruikers toegewezen, maar de installatie is mislukt. '
  
- Dit kan gebeuren als een enkelvoudige VPP-token wordt gebruikt in meerdere providers voor het beheer van mobiele apparaten. VPP-tokens van Apple mogen enkel worden gebruikt voor één provider. Als u een VPP-token met meerdere providers hebt gebruikt, moet u het token opnieuw uploaden naar intune.

- De installatie kan ook mislukken als het totale aantal installaties groter is dan het aantal licenties. Als u een gebruiksrapport voor uw licenties wilt weergeven, gaat u naar de pagina licenties van de apps voor **mobiele apps intune** \> **App licenses** . Zie [dit artikel](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens) voor meer informatie over het opnieuw claimen van licenties die in gebruik zijn.
