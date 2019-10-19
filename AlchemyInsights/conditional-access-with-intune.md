---
title: Voorwaardelijke toegang met intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504989"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="d1093-102">Voorwaardelijke toegang met intune</span><span class="sxs-lookup"><span data-stu-id="d1093-102">Conditional Access with Intune</span></span>

<span data-ttu-id="d1093-103">Het gebruik van **voorwaardelijke toegang** met intune vereist 3 stappen:</span><span class="sxs-lookup"><span data-stu-id="d1093-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="d1093-104">Maak een **beleid voor voorwaardelijke toegang** waarin wordt gedefinieerd welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze resources.</span><span class="sxs-lookup"><span data-stu-id="d1093-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="d1093-105">Een apparaat moet bijvoorbeeld compatibel zijn voordat u toegang tot zakelijke e-mail.</span><span class="sxs-lookup"><span data-stu-id="d1093-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="d1093-106">Maak een **nalevingsbeleid** om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="d1093-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="d1093-107">Een apparaat moet bijvoorbeeld een pincode hebben van ten minste 6 cijfers voordat het als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="d1093-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="d1093-108">Ervoor te zorgen dat zowel **nalevingsbeleid** en **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="d1093-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="d1093-109">Dit kan nodig zijn voor het maken van specifieke groepen gebruikers in azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1093-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="d1093-110">Lees meer:</span><span class="sxs-lookup"><span data-stu-id="d1093-110">Read more:</span></span>
  
- [<span data-ttu-id="d1093-111">Aanbevolen procedures voor voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="d1093-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="d1093-112">Aan de slag met voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="d1093-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

