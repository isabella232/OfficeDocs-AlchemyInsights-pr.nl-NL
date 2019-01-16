---
title: Werken met iOS VPP toepassingen regel Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284719"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="123c0-102">Werken met iOS VPP-toepassingen</span><span class="sxs-lookup"><span data-stu-id="123c0-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="123c0-103">[IOS apps hebt aangeschaft via een volume inkoop programma met Microsoft Intune beheren](https://docs.microsoft.com/intune/vpp-apps-ios) voor meer informatie over functies, beperkingen en stappen om te lezen van een Apple Volume inkoop en de ondersteuning voor het Microsoft Intune gebruiken.</span><span class="sxs-lookup"><span data-stu-id="123c0-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="123c0-104">**Problemen:** "Ik heb een VPP iOS app Mijn gebruikers toegewezen, maar de installatie is mislukt."</span><span class="sxs-lookup"><span data-stu-id="123c0-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="123c0-p101">Dit kan gebeuren als een enkele VPP-token wordt gebruikt in meerdere providers van mobiele apparaat beheer. VPP tokens van Apple kunnen alleen worden gebruikt met één provider. Als u een token VPP met meerdere providers gebruikt, moet u de Intune-token opnieuw uploaden.</span><span class="sxs-lookup"><span data-stu-id="123c0-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="123c0-p102">De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt. Een gebruiksrapport voor uw licenties, Ga naar de **Intune Mobile apps** \> **App licenties** pagina. Als u wilt weten hoe u licenties gebruikt, vrijkomt, Zie [in dit artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="123c0-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

