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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420479"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="aecef-102">Werken met iOS VPP-toepassingen</span><span class="sxs-lookup"><span data-stu-id="aecef-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="aecef-103">[IOS apps hebt aangeschaft via een volume inkoop programma met Microsoft Intune beheren](https://docs.microsoft.com/intune/vpp-apps-ios) voor meer informatie over functies, beperkingen en stappen om te lezen van een Apple Volume inkoop en de ondersteuning voor het Microsoft Intune gebruiken.</span><span class="sxs-lookup"><span data-stu-id="aecef-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="aecef-104">**Problemen:** "Ik heb een VPP iOS app Mijn gebruikers toegewezen, maar de installatie is mislukt."</span><span class="sxs-lookup"><span data-stu-id="aecef-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="aecef-105">Dit kan gebeuren als een enkele VPP-token wordt gebruikt in meerdere providers van mobiele apparaat beheer.</span><span class="sxs-lookup"><span data-stu-id="aecef-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="aecef-106">VPP tokens van Apple kunnen alleen worden gebruikt met één provider.</span><span class="sxs-lookup"><span data-stu-id="aecef-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="aecef-107">Als u een token VPP met meerdere providers gebruikt, moet u de Intune-token opnieuw uploaden.</span><span class="sxs-lookup"><span data-stu-id="aecef-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="aecef-108">De installatie kan ook mislukken als het totale aantal installaties het aantal licenties overschrijdt.</span><span class="sxs-lookup"><span data-stu-id="aecef-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="aecef-109">Een gebruiksrapport voor uw licenties, Ga naar de **Intune Mobile apps** \> **App licenties** pagina.</span><span class="sxs-lookup"><span data-stu-id="aecef-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="aecef-110">Als u wilt weten hoe u licenties gebruikt, vrijkomt, Zie [in dit artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="aecef-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

