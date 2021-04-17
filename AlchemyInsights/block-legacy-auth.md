---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820173"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="3d58c-102">Oudere verificatie blokkeren</span><span class="sxs-lookup"><span data-stu-id="3d58c-102">Blocking legacy authentication</span></span>

<span data-ttu-id="3d58c-103">Oudere verificatie is een term die verwijst naar een verificatieaanvraag die wordt gedaan door:</span><span class="sxs-lookup"><span data-stu-id="3d58c-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="3d58c-104">Oudere Office-clients die geen moderne verificatie gebruiken (bijvoorbeeld Office 2010-client).</span><span class="sxs-lookup"><span data-stu-id="3d58c-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="3d58c-105">Elke client die oudere e-mailprotocollen gebruikt, zoals IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="3d58c-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="3d58c-106">Zie Oudere verificatie blokkeren voor meer informatie over het blokkeren van oudere verificatie en het inschakelen van moderne [verificatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="3d58c-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="3d58c-107">Beveiligingsinstellingen in Azure Active Directory (Azure AD) maken het gemakkelijker om veilig te zijn en uw organisatie te beschermen.</span><span class="sxs-lookup"><span data-stu-id="3d58c-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="3d58c-108">Beveiligingsinstellingen bevatten vooraf geconfigureerde beveiligingsinstellingen voor veelvoorkomende aanvallen.</span><span class="sxs-lookup"><span data-stu-id="3d58c-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="3d58c-109">Zie Wat [zijn beveiligingsinstellingen?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)voor meer informatie over beveiligingsinstellingen.</span><span class="sxs-lookup"><span data-stu-id="3d58c-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="3d58c-110">**Opmerking:** Als uw tenant is gemaakt op of na 22 oktober 2019, is het mogelijk dat u te maken krijgt met het nieuwe beveiligingsgedrag en dat er al beveiligings defaults zijn ingeschakeld in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="3d58c-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="3d58c-111">In een poging om al onze gebruikers te beschermen, worden beveiligingsinstellingen uitgerold naar alle nieuwe tenants die zijn gemaakt.</span><span class="sxs-lookup"><span data-stu-id="3d58c-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
