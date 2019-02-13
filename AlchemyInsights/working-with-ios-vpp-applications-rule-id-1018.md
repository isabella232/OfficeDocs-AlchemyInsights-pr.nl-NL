---
title: Werken met iOS VPP toepassingen regel Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917491"
---
# <a name="working-with-ios-vpp-applications"></a>Werken met iOS VPP-toepassingen

[IOS apps hebt aangeschaft via een volume inkoop programma met Microsoft Intune beheren](https://docs.microsoft.com/intune/vpp-apps-ios) voor meer informatie over functies, beperkingen en stappen om te lezen van een Apple Volume inkoop en de ondersteuning voor het Microsoft Intune gebruiken. 
  
 **Problemen:** "Ik heb een VPP iOS app Mijn gebruikers toegewezen, maar de installatie is mislukt." 
  
- Dit kan gebeuren als een enkele VPP-token wordt gebruikt in meerdere providers van mobiele apparaat beheer. VPP tokens van Apple kunnen alleen worden gebruikt met één provider. Als u een token VPP met meerdere providers gebruikt, moet u de Intune-token opnieuw uploaden.
    
- De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt. Een gebruiksrapport voor uw licenties, Ga naar de **Intune Mobile apps** \> **App licenties** pagina. Als u wilt weten hoe u licenties gebruikt, vrijkomt, Zie [in dit artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

