---
title: API-machtigingen en toestemming
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974372"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="e9f5a-102">API-machtigingen en toestemming</span><span class="sxs-lookup"><span data-stu-id="e9f5a-102">API permissions and consent</span></span>

<span data-ttu-id="e9f5a-103">Toepassingen die worden geïntegreerd met Microsoft Identity platform volgen een machtigings model waarmee gebruikers en beheerders kunnen bepalen hoe gegevens kunnen worden geopend.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="e9f5a-104">De implementatie van het autorisatie model is bijgewerkt op het Microsoft Identity platform-eindpunt.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="e9f5a-105">De werking van een app moet werken met Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="e9f5a-106">[Machtigingen en instemming in het eindpunt van Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) zijn belangrijke basisprincipes van dit autorisatie model, waaronder scopes, machtigingen en toestemming.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="e9f5a-107">Met het [toestemmings raamwerk van Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) kunt u eenvoudig webtoepassingen voor meerdere tenants en native clienttoepassingen ontwikkelen.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="e9f5a-108">Deze toepassingen kunnen zich aanmelden bij gebruikersaccounts van een Azure AD-Tenant die verschilt van het abonnement waar de toepassing is geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="e9f5a-109">Het is mogelijk dat u ook Web-Api's nodig hebt, zoals de Microsoft Graph API (voor toegang tot Azure AD, intune en services in Microsoft 365) en andere Api's van Microsoft-services, naast uw eigen web-Api's.</span><span class="sxs-lookup"><span data-stu-id="e9f5a-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

