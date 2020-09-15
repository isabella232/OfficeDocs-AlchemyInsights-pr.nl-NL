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
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="01ca2-102">Werken met VPP-toepassingen van iOS</span><span class="sxs-lookup"><span data-stu-id="01ca2-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="01ca2-103">Meer informatie over het [beheren van Ios-apps die u hebt gekocht via een volume aankoopprogramma met Microsoft intune](https://docs.microsoft.com/intune/vpp-apps-ios) voor informatie over functies, beperkingen en stappen voor het gebruik van het Apple volume Purchase Program en de ondersteuning hiervan in Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="01ca2-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="01ca2-104">**Veelvoorkomende problemen:** ' Ik heb een iOS VPP-app aan mijn gebruikers toegewezen, maar de installatie is mislukt. '</span><span class="sxs-lookup"><span data-stu-id="01ca2-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="01ca2-105">Dit kan gebeuren als een enkelvoudige VPP-token wordt gebruikt in meerdere providers voor het beheer van mobiele apparaten.</span><span class="sxs-lookup"><span data-stu-id="01ca2-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="01ca2-106">VPP-tokens van Apple mogen enkel worden gebruikt voor één provider.</span><span class="sxs-lookup"><span data-stu-id="01ca2-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="01ca2-107">Als u een VPP-token met meerdere providers hebt gebruikt, moet u het token opnieuw uploaden naar intune.</span><span class="sxs-lookup"><span data-stu-id="01ca2-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="01ca2-108">De installatie kan ook mislukken als het totale aantal installaties groter is dan het aantal licenties.</span><span class="sxs-lookup"><span data-stu-id="01ca2-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="01ca2-109">Als u een gebruiksrapport voor uw licenties wilt weergeven, gaat u naar de pagina licenties van de apps voor **mobiele apps intune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="01ca2-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="01ca2-110">Zie [dit artikel](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens) voor meer informatie over het opnieuw claimen van licenties die in gebruik zijn.</span><span class="sxs-lookup"><span data-stu-id="01ca2-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
