---
title: Er is een fout opgetreden bij het valideren van toegangstoken fout tijdens het on-boarding van Desktop Analytics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741154"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="0f8ad-102">Foutbericht ' er is een fout bij het valideren van toegangstoken ' tijdens het onboarding van Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="0f8ad-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="0f8ad-103">Deze fout wordt meestal waargenomen wanneer het verificatietoken is verlopen.</span><span class="sxs-lookup"><span data-stu-id="0f8ad-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="0f8ad-104">Normaalgesproken vernieuwen van de pagina wordt het token vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="0f8ad-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="0f8ad-105">Dit probleem kan echter blijven bestaan als er beleid voor voorwaardelijke toegang is toegepast op het account dat wordt gebruikt voor on-Board Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="0f8ad-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="0f8ad-106">U de Azure AD-aanmelding in de logboeken in de Azure-Portal om te zien of er fouten optreden voor het account dat wordt gebruikt voor de onboarding van Desktop Analytics controleren.</span><span class="sxs-lookup"><span data-stu-id="0f8ad-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="0f8ad-107">Ga naar de [implementatie van uw voorwaardelijke toegang plannen](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)voor meer informatie over voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="0f8ad-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>