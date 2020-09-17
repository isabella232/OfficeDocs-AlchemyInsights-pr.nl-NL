---
title: Er is een fout opgetreden bij het valideren van een toegangstoken fout tijdens de bureaublad analyse op het bord
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783546"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="45a46-102">Fout ' er is een fout opgetreden bij het valideren van een toegangstoken ' tijdens de bureaublad analyse</span><span class="sxs-lookup"><span data-stu-id="45a46-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="45a46-103">Deze fout wordt normaal geconstateerd wanneer het authenticatietoken verloopt.</span><span class="sxs-lookup"><span data-stu-id="45a46-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="45a46-104">Meestal wordt de token vernieuwd wanneer u de pagina vernieuwt.</span><span class="sxs-lookup"><span data-stu-id="45a46-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="45a46-105">Dit probleem kan echter zich voordoen als er voorwaardelijke toegangsbeleidsregels gelden voor het account dat wordt gebruikt voor de on-board Analytics Desk.</span><span class="sxs-lookup"><span data-stu-id="45a46-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="45a46-106">U kunt de aanmeldingslogboeken van Azure AD in de Azure-Portal bekijken om te zien of er aanmeldingsfouten zijn voor het account dat wordt gebruikt voor het onboarden van bureaublad analyses.</span><span class="sxs-lookup"><span data-stu-id="45a46-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="45a46-107">Ga naar [uw implementatie voor voorwaardelijke toegang plannen](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)voor meer informatie over voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="45a46-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>