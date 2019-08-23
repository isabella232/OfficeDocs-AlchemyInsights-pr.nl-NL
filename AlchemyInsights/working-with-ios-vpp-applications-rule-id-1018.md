---
title: Werken met iOS VPP toepassingen regel Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557984"
---
# <a name="working-with-ios-vpp-applications"></a>Werken met iOS VPP-toepassingen

[IOS apps hebt aangeschaft via een volume inkoop programma met Microsoft Intune beheren](https://docs.microsoft.com/intune/vpp-apps-ios) voor meer informatie over functies, beperkingen en stappen om te lezen van een Apple Volume inkoop en de ondersteuning voor het Microsoft Intune gebruiken.
  
 **Problemen:** "Ik heb een VPP iOS app Mijn gebruikers toegewezen, maar de installatie is mislukt."
  
- Dit kan gebeuren als een enkele VPP-token wordt gebruikt in meerdere providers van mobiele apparaat beheer. VPP tokens van Apple kunnen alleen worden gebruikt met één provider. Als u een token VPP met meerdere providers gebruikt, moet u de Intune-token opnieuw uploaden.

- De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt. Een gebruiksrapport voor uw licenties, Ga naar de **Intune Mobile apps** \> **App licenties** pagina. Als u wilt weten hoe u licenties gebruikt, vrijkomt, Zie [in dit artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
