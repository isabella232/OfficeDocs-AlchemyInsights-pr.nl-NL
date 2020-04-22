---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706016"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="5f3ce-102">Voorwaardelijke toegang met Intune</span><span class="sxs-lookup"><span data-stu-id="5f3ce-102">Conditional Access with Intune</span></span>

<span data-ttu-id="5f3ce-103">Het gebruik **van voorwaardelijke toegang** met Intune vereist 3 stappen:</span><span class="sxs-lookup"><span data-stu-id="5f3ce-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="5f3ce-104">Maak een **beleid voor voorwaardelijke toegang** waarin wordt gedefinieerd welke resources worden beschermd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze bronnen.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="5f3ce-105">Een apparaat moet bijvoorbeeld compatibel zijn voordat het bedrijfse-mail inziet.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="5f3ce-106">Maak een **nalevingsbeleid** om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="5f3ce-107">Een apparaat moet bijvoorbeeld een pin van ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="5f3ce-108">Ervoor zorgen dat zowel **nalevingsbeleid** als **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="5f3ce-109">Hiervoor moeten mogelijk specifieke groepen gebruikers worden gemaakt in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="5f3ce-110">Lees meer:</span><span class="sxs-lookup"><span data-stu-id="5f3ce-110">Read more:</span></span>
  
- [<span data-ttu-id="5f3ce-111">Aanbevolen procedures voor voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="5f3ce-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="5f3ce-112">Aan de slag met voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="5f3ce-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

