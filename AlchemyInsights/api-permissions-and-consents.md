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
# <a name="api-permissions-and-consent"></a>API-machtigingen en toestemming

Toepassingen die worden geïntegreerd met Microsoft Identity platform volgen een machtigings model waarmee gebruikers en beheerders kunnen bepalen hoe gegevens kunnen worden geopend. De implementatie van het autorisatie model is bijgewerkt op het Microsoft Identity platform-eindpunt. De werking van een app moet werken met Microsoft Identity platform. [Machtigingen en instemming in het eindpunt van Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) zijn belangrijke basisprincipes van dit autorisatie model, waaronder scopes, machtigingen en toestemming.

Met het [toestemmings raamwerk van Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) kunt u eenvoudig webtoepassingen voor meerdere tenants en native clienttoepassingen ontwikkelen. Deze toepassingen kunnen zich aanmelden bij gebruikersaccounts van een Azure AD-Tenant die verschilt van het abonnement waar de toepassing is geregistreerd. Het is mogelijk dat u ook Web-Api's nodig hebt, zoals de Microsoft Graph API (voor toegang tot Azure AD, intune en services in Microsoft 365) en andere Api's van Microsoft-services, naast uw eigen web-Api's.

