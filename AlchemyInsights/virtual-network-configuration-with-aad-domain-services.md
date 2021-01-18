---
title: Virtuele configuratie met AAD-domeinservices
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884977"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="62ee5-102">Virtuele configuratie met AAD-domeinservices</span><span class="sxs-lookup"><span data-stu-id="62ee5-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="62ee5-103">Virtuele configuratie met AAD-domein service omvat de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="62ee5-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="62ee5-104">De status van uw domein controleren op de Azure-Portal https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="62ee5-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="62ee5-105">Controleren van uw NSG voor regels waarmee de benodigde poorten voor synchronisatie in azure AD Domain Services op de portal worden geblokkeerd https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="62ee5-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="62ee5-106">Zorg ervoor dat uw virtuele netwerk in hetzelfde Azure-gebied is geïmplementeerd als uw Azure AD Domain Services-beheerd domein.</span><span class="sxs-lookup"><span data-stu-id="62ee5-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="62ee5-107">Zorg ervoor dat u geen bestaand domein hebt met dezelfde domeinnaam die beschikbaar is in het virtuele netwerk.</span><span class="sxs-lookup"><span data-stu-id="62ee5-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="62ee5-108">Zie voor meer informatie over het ontwerpen van de aandacht op het [virtuele netwerk van](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)Azure voor ondersteuning voor Aad Domain Services.</span><span class="sxs-lookup"><span data-stu-id="62ee5-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

