---
title: API-machtigingen en -toestemming
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932092"
---
# <a name="api-permissions-and-consent"></a>API-machtigingen en toestemming

Toepassingen die met een Microsoft identity platform worden geïntegreerd, volgen een autorisatiemodel dat gebruikers en beheerders controle geeft over hoe gegevens kunnen worden gebruikt. De implementatie van het autorisatiemodel is bijgewerkt op het Microsoft identity platform eindpunt. De manier waarop een app moet werken met de Microsoft identity platform. [Machtigingen en toestemming in](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Microsoft identity platform eindpunt hebben betrekking op de basisbegrippen van dit autorisatiemodel, inclusief scopes, machtigingen en toestemming.

Met [Azure Active Directory (Azure AD)-toestemmingskader](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) kunt u eenvoudig web- en native clienttoepassingen met meerdere tenants ontwikkelen. Met deze toepassingen kunt u zich aanmelden door gebruikersaccounts van een Azure AD-tenant die verschilt van de tenant waarin de toepassing is geregistreerd. Ze hebben mogelijk ook toegang nodig tot web-API's, zoals de Microsoft Graph-API (voor toegang tot Azure AD, Intune en services in Microsoft 365) en andere API's van Microsoft-services, naast uw eigen web-API's.

