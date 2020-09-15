---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685593"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="49598-102">Verouderde authenticatie blokkeren</span><span class="sxs-lookup"><span data-stu-id="49598-102">Blocking legacy authentication</span></span>

<span data-ttu-id="49598-103">Oudere verificatie is een term die verwijst naar een verificatieaanvraag die is gemaakt door:</span><span class="sxs-lookup"><span data-stu-id="49598-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="49598-104">Oudere Office-clients die geen moderne verificatie gebruiken, bijvoorbeeld Office 2010-client.</span><span class="sxs-lookup"><span data-stu-id="49598-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="49598-105">Elke client die gebruikmaakt van oudere e-mail protocollen, zoals IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="49598-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="49598-106">Zie voor meer informatie over het blokkeren van oudere verificatie en het inschakelen van moderne verificatie de mogelijkheid om [oudere verificatie te blokkeren](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="49598-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="49598-107">Met behulp van beveiligingsstandaarden in azure Active Directory (Azure AD) kunt u eenvoudiger veilig zijn en uw organisatie beschermen.</span><span class="sxs-lookup"><span data-stu-id="49598-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="49598-108">Beveiligingsstandaard waarden bevatten vooraf geconfigureerde beveiligingsinstellingen voor algemene aanvallen.</span><span class="sxs-lookup"><span data-stu-id="49598-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="49598-109">Zie voor meer informatie over beveiligingsstandaarden: [Wat zijn beveiligingsstandaarden?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="49598-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="49598-110">**Opmerking**: als de Tenant is gemaakt op of na de 22 van oktober 2019, is het mogelijk dat u het nieuwe beveiligde standaardgedrag hebt en dat de standaardinstellingen voor beveiliging al zijn ingeschakeld in uw Tenant.</span><span class="sxs-lookup"><span data-stu-id="49598-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="49598-111">Als u alle gebruikers wilt beschermen, worden de beveiligingsstandaard waarden voor alle nieuwe tenants gemaakt.</span><span class="sxs-lookup"><span data-stu-id="49598-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
