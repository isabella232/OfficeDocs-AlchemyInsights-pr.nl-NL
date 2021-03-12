---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704781"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="2403f-102">Voorwaardelijke toegang met Intune</span><span class="sxs-lookup"><span data-stu-id="2403f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="2403f-103">Voor  **het gebruik van**  voorwaardelijke toegang met Intune zijn drie stappen vereist:</span><span class="sxs-lookup"><span data-stu-id="2403f-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="2403f-104">Maak een  **compliancebeleid** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)om instellingen te definiëren die moeten worden voldaan voordat het apparaat als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="2403f-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="2403f-105">Een apparaat moet bijvoorbeeld een pincode met ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd.</span><span class="sxs-lookup"><span data-stu-id="2403f-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="2403f-106">Maak een **beleid voor voorwaardelijke**  toegang dat bepaalt welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan voor toegang tot deze bronnen.</span><span class="sxs-lookup"><span data-stu-id="2403f-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="2403f-107">[Een apparaat moet bijvoorbeeld](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  compatibel zijn voordat u zakelijke e-mail kunt openen.</span><span class="sxs-lookup"><span data-stu-id="2403f-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="2403f-108">Zorg ervoor **dat zowel het nalevingsbeleid**  als het beleid  **voor**  voorwaardelijke toegang zijn gericht op de gewenste groepen gebruikers.</span><span class="sxs-lookup"><span data-stu-id="2403f-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="2403f-109">Hiervoor moet u mogelijk specifieke groepen gebruikers maken in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2403f-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="2403f-110">**Handige koppelingen:**</span><span class="sxs-lookup"><span data-stu-id="2403f-110">**Helpful links:**</span></span>

[<span data-ttu-id="2403f-111">Overzicht van apparaat compliance</span><span class="sxs-lookup"><span data-stu-id="2403f-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="2403f-112">Problemen met CA oplossen</span><span class="sxs-lookup"><span data-stu-id="2403f-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="2403f-113">Beleid voor probleemoplossing</span><span class="sxs-lookup"><span data-stu-id="2403f-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="2403f-114">Als u e-mail (Exchange Online) wilt beveiligen tegen toegang door niet-compatibele apparaten, moeten beide documenten worden gevolgd:</span><span class="sxs-lookup"><span data-stu-id="2403f-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="2403f-115">E-mailtoegang beveiligen tegen apparaten met EAS</span><span class="sxs-lookup"><span data-stu-id="2403f-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="2403f-116">E-mailtoegang beveiligen tegen apparaten met moderne verificatie-clients zoals Outlook</span><span class="sxs-lookup"><span data-stu-id="2403f-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)