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
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931425"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1ce83-102">Voorwaardelijke toegang met Intune</span><span class="sxs-lookup"><span data-stu-id="1ce83-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1ce83-103">Als u **Voorwaardelijke toegang** met Intune gebruikt, zijn 3 stappen vereist:</span><span class="sxs-lookup"><span data-stu-id="1ce83-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="1ce83-104">Maak een **nalevingsbeleid** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="1ce83-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1ce83-105">Een apparaat moet bijvoorbeeld een pin van ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="1ce83-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="1ce83-106">Maak een **beleid voor voorwaardelijke toegang** dat bepaalt welke resources worden beschermd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze bronnen.</span><span class="sxs-lookup"><span data-stu-id="1ce83-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="1ce83-107">[Een](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) apparaat moet bijvoorbeeld compatibel zijn voordat het toegang krijgt tot zakelijke e-mail.</span><span class="sxs-lookup"><span data-stu-id="1ce83-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="1ce83-108">Zorg ervoor dat zowel **nalevingsbeleid** als **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="1ce83-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="1ce83-109">Hiervoor moeten mogelijk specifieke groepen gebruikers in Azure Active Directory worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="1ce83-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="1ce83-110">**Nuttige links:**</span><span class="sxs-lookup"><span data-stu-id="1ce83-110">**Helpful links:**</span></span>

[<span data-ttu-id="1ce83-111">Overzicht van apparaatnaleving</span><span class="sxs-lookup"><span data-stu-id="1ce83-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="1ce83-112">Problemen met CA oplossen</span><span class="sxs-lookup"><span data-stu-id="1ce83-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1ce83-113">Probleemoplossingsbeleid</span><span class="sxs-lookup"><span data-stu-id="1ce83-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="1ce83-114">Om e-mail (Exchange online) te beschermen tegen toegang door niet-compatibele apparaten, moeten beide documenten worden gevolgd:</span><span class="sxs-lookup"><span data-stu-id="1ce83-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="1ce83-115">E-mailtoegang beschermen tegen apparaten met EAS</span><span class="sxs-lookup"><span data-stu-id="1ce83-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="1ce83-116">E-mailtoegang beveiligen tegen apparaten met behulp van moderne verificatieclients zoals Outlook</span><span class="sxs-lookup"><span data-stu-id="1ce83-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)