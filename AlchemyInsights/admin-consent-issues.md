---
title: Problemen met beheerders instemming
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900929"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="fc6bc-102">Problemen met beheerders instemming</span><span class="sxs-lookup"><span data-stu-id="fc6bc-102">Admin consent issues</span></span>

1. <span data-ttu-id="fc6bc-103">Schakel de [beheerder toestemming](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) voor het doorgeven van beheerders rechtstreeks vanuit het scherm voor toestemming in.</span><span class="sxs-lookup"><span data-stu-id="fc6bc-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="fc6bc-104">Zie het volgende artikel voor de stappen voor probleemoplossing: [onverwachte fout bij het uitvoeren van een aanvraag voor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)het oplossen van problemen wanneer gebruikers van de toepassing onverwachte fouten zien tijdens het toestemming proces.</span><span class="sxs-lookup"><span data-stu-id="fc6bc-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="fc6bc-105">Meer informatie over [beheerders aanvragen voor het Microsoft-identiteits platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), de werking van de [instemming](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) en de [beoordeling van een aanvraag voor de beheerders vergunning voor de gehele Tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="fc6bc-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="fc6bc-106">Toepassingen die worden geïntegreerd met Microsoft Identity platform volgen een machtigings model waarmee gebruikers en beheerders kunnen bepalen hoe gegevens kunnen worden geopend.</span><span class="sxs-lookup"><span data-stu-id="fc6bc-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="fc6bc-107">De implementatie van het autorisatie model op het Microsoft Identity platform-eindpunt is bijgewerkt en de manier waarop een app moet communiceren met het Microsoft-identiteits platform.</span><span class="sxs-lookup"><span data-stu-id="fc6bc-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="fc6bc-108">Zie [machtigingen en instemming in het eindpunt van Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) voor een overzicht van dit autorisatie model, waaronder bereiken, machtigingen en toestemming.</span><span class="sxs-lookup"><span data-stu-id="fc6bc-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>