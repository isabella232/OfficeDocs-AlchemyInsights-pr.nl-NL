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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504989"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a989c-102">Voorwaardelijke toegang met Intune</span><span class="sxs-lookup"><span data-stu-id="a989c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a989c-103">Met behulp van **Voorwaardelijke toegang** met Intune vereist 3 stappen:</span><span class="sxs-lookup"><span data-stu-id="a989c-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="a989c-104">Maak een **Voorwaardelijke-beleid** waarmee wordt gedefinieerd welke bronnen zijn beveiligd en voorwaarden moeten worden voldaan voor toegang tot deze bronnen.</span><span class="sxs-lookup"><span data-stu-id="a989c-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="a989c-105">Bijvoorbeeld moet een apparaat voldoen voor toegang tot zakelijke e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="a989c-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="a989c-106">Maak een **Naleving van beleid** om te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="a989c-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="a989c-107">Een apparaat moet bijvoorbeeld een pincode van ten minste 6 cijfers hebben, voordat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="a989c-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="a989c-108">Ervoor te zorgen dat **Zowel naleving van beleidsregels** en **voorwaardelijke toegang** gericht zijn op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="a989c-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="a989c-109">Hiervoor kunnen specifieke groepen gebruikers maken in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a989c-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="a989c-110">Lees meer:</span><span class="sxs-lookup"><span data-stu-id="a989c-110">Read more:</span></span>
  
- [<span data-ttu-id="a989c-111">Aanbevolen procedures voor voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="a989c-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="a989c-112">Aan de slag met voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="a989c-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

