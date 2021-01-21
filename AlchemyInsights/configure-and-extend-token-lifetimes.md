---
title: Levensduur van tokens configureren en verlengen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916824"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="cf492-102">Levensduur van tokens configureren en verlengen</span><span class="sxs-lookup"><span data-stu-id="cf492-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="cf492-103">U kunt de levensduur opgeven van een toegangs-, SAML-of ID-token dat is uitgegeven door Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="cf492-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="cf492-104">U kunt token levensduur instellen voor alle apps in uw organisatie, voor een toepassing via meerdere tenants of voor een bepaalde service-principal in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="cf492-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="cf492-105">Voor meer informatie raadpleegt u de [levensduur van configureerbare tokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="cf492-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="cf492-106">Zie voorbeelden [van de levensduur van tokens configureren](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)voor voorbeelden.</span><span class="sxs-lookup"><span data-stu-id="cf492-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="cf492-107">Zie [tokens configureren in azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)voor informatie over het configureren van de levensduur en de compatibiliteit van een token in azure Active Directory B2C (Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="cf492-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="cf492-108">In het artikel wordt het gedrag van de verbinding voor eenmalige aanmelding (SSO) van Azure [Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beschreven en kunt u de meest geschikte SSO-methode kiezen wanneer u uw beleid configureert.</span><span class="sxs-lookup"><span data-stu-id="cf492-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="cf492-109">**Hoelang duurt het zo lang? Hoelang zijn ze geldig?**</span><span class="sxs-lookup"><span data-stu-id="cf492-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="cf492-110">Levensduur van tokens zijn 1 uur en de levensduur van een sessie is 24 uur.</span><span class="sxs-lookup"><span data-stu-id="cf492-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="cf492-111">Dit betekent dat als er geen aanvragen binnen 24 uur zijn ingediend, u opnieuw moet inloggen voordat u een nieuw token aanvraagt.</span><span class="sxs-lookup"><span data-stu-id="cf492-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="cf492-112">Na 30 mei 2020 kan geen nieuwe Tenant gebruikmaken van het beleid voor de levenscyclus van configureerbare tokens om sessie-en vernieuwingstokens te configureren.</span><span class="sxs-lookup"><span data-stu-id="cf492-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="cf492-113">De afschaffing valt binnen enkele maanden, wat betekent dat we niet meer voldoen aan bestaande sessies en vernieuwingstokens.</span><span class="sxs-lookup"><span data-stu-id="cf492-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="cf492-114">U kunt de levensduur van toegangstokens na de afschaffing nog steeds configureren.</span><span class="sxs-lookup"><span data-stu-id="cf492-114">You can still configure access token lifetimes after the deprecation.</span></span>






