---
title: Voorwaardelijke toegang gebruiken met Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692975"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="7fd2c-102">Voorwaardelijke toegang gebruiken met Intune</span><span class="sxs-lookup"><span data-stu-id="7fd2c-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="7fd2c-103">Voor het gebruik van voorwaardelijke toegang met Intune zijn drie stappen vereist:</span><span class="sxs-lookup"><span data-stu-id="7fd2c-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="7fd2c-104">Maak een compliancebeleid om instellingen te definiëren die moeten worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pincode met ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="7fd2c-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="7fd2c-105">Maak een beleid voor voorwaardelijke toegang dat bepaalt welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan voor toegang tot deze bronnen. Een apparaat moet bijvoorbeeld compatibel zijn voordat u zakelijke e-mail kunt openen.</span><span class="sxs-lookup"><span data-stu-id="7fd2c-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="7fd2c-106">Zorg ervoor dat zowel het nalevingsbeleid als het beleid voor voorwaardelijke toegang zijn gericht op de gewenste groepen gebruikers. Hiervoor moet u mogelijk specifieke groepen gebruikers maken in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7fd2c-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7fd2c-107">Meer informatie...</span><span class="sxs-lookup"><span data-stu-id="7fd2c-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
