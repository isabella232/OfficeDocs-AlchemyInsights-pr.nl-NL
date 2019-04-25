---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393536"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c13ef-102">Voorwaardelijke toegang met Intune</span><span class="sxs-lookup"><span data-stu-id="c13ef-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c13ef-103">Met behulp van **Voorwaardelijke toegang** met Intune vereist 3 stappen:</span><span class="sxs-lookup"><span data-stu-id="c13ef-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c13ef-104">Maak een **Voorwaardelijke-beleid** waarmee wordt gedefinieerd welke bronnen zijn beveiligd en voorwaarden moeten worden voldaan voor toegang tot deze bronnen.</span><span class="sxs-lookup"><span data-stu-id="c13ef-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="c13ef-105">Bijvoorbeeld moet een apparaat voldoen voor toegang tot zakelijke e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="c13ef-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c13ef-106">Maak een **Naleving van beleid** om te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="c13ef-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c13ef-107">Een apparaat moet bijvoorbeeld een pincode van ten minste 6 cijfers hebben, voordat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="c13ef-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c13ef-108">Ervoor te zorgen dat **Zowel naleving van beleidsregels** en **voorwaardelijke toegang** gericht zijn op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="c13ef-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="c13ef-109">Hiervoor kunnen specifieke groepen gebruikers maken in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c13ef-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c13ef-110">Lees meer:</span><span class="sxs-lookup"><span data-stu-id="c13ef-110">Read more:</span></span>
  
- [<span data-ttu-id="c13ef-111">Aanbevolen procedures voor voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="c13ef-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c13ef-112">Aan de slag met voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="c13ef-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

