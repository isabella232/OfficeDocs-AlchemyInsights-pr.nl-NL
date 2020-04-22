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
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="a3b1e-102">Werken met iOS VPP-toepassingen</span><span class="sxs-lookup"><span data-stu-id="a3b1e-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="a3b1e-103">Lees [Hoe u iOS-apps beheert die zijn aangeschaft via een programma voor volumeaankoop met Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) om meer te weten te komen over functies, beperkingen en stappen om gebruik te maken van het Apple Volume Purchase Program en de ondersteuning hiervoor in Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="a3b1e-104">**Veelvoorkomende problemen:** "Ik heb een iOS VPP-app toegewezen aan mijn gebruikers, maar de installatie is mislukt."</span><span class="sxs-lookup"><span data-stu-id="a3b1e-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="a3b1e-105">Dit kan gebeuren als één VPP-token wordt gebruikt voor meerdere providers voor het beheer van mobiele apparaten.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="a3b1e-106">VPP-tokens van Apple mogen slechts bij één provider worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="a3b1e-107">Als u een VPP-token met meerdere providers hebt gebruikt, moet u het token opnieuw uploaden naar Intune.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="a3b1e-108">De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="a3b1e-109">Als u een gebruiksrapport voor uw licenties wilt bekijken, gaat u naar de pagina **Licenties voor Apps-apps** **inAfstemmen.** \></span><span class="sxs-lookup"><span data-stu-id="a3b1e-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="a3b1e-110">Zie dit artikel voor meer informatie over het terugvorderen van licenties die in gebruik [zijn.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="a3b1e-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
