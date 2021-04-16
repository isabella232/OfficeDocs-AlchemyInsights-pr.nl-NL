---
title: Er is een fout opgetreden bij het valideren van toegangs token tijdens het instappen in Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813683"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="506e1-102">Fout 'Er is een fout opgetreden bij het valideren van toegangs-token' tijdens de onboarding van Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="506e1-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="506e1-103">Deze fout wordt normaal gesproken waargenomen wanneer het verificatie-token verloopt.</span><span class="sxs-lookup"><span data-stu-id="506e1-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="506e1-104">Meestal wordt het token vernieuwd door de pagina te vernieuwen.</span><span class="sxs-lookup"><span data-stu-id="506e1-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="506e1-105">Dit probleem kan echter blijven bestaan als er beleid voor voorwaardelijke toegang is toegepast op het account dat wordt gebruikt voor desktopanalyse aan boord.</span><span class="sxs-lookup"><span data-stu-id="506e1-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="506e1-106">U kunt de Aanmeldingslogboeken voor Azure AD bekijken in de Azure Portal om te zien of er aanmeldingsfouten zijn voor het account dat wordt gebruikt voor de onboarding van Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="506e1-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="506e1-107">Ga naar Voorwaardelijke toegang plannen voor meer informatie over voorwaardelijke [toegang.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="506e1-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>