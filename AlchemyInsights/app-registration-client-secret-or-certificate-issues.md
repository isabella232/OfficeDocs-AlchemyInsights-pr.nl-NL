---
title: App Registration Client Secret or Certificate issues
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404459"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="0dd5e-102">App Registration Client Secret or Certificate issues</span><span class="sxs-lookup"><span data-stu-id="0dd5e-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="0dd5e-103">Verloopt het geheim van de toepassingsclient?</span><span class="sxs-lookup"><span data-stu-id="0dd5e-103">Application client secret expiring?</span></span>

<span data-ttu-id="0dd5e-104">Ongeacht hoe de geregistreerde toepassing is gemaakt, hetzij via het standaardregistratieproces in de app-registratieportal of als de serviceprincipaal in uw tenant is gemaakt met toepassings toestemming, moet er een nieuwe clientgeheim worden gemaakt vóór het verlopen van de huidige toepassing en worden bijgewerkt in de bijbehorende toepassingscode.</span><span class="sxs-lookup"><span data-stu-id="0dd5e-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="0dd5e-105">De maximale geldigheidsduur is 2 jaar.</span><span class="sxs-lookup"><span data-stu-id="0dd5e-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="0dd5e-106">Ter herinnering: de geheime waarde moet worden opgenomen omdat deze niet meer zichtbaar is nadat u de pagina App-registraties in de portal hebt verlaten.</span><span class="sxs-lookup"><span data-stu-id="0dd5e-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="0dd5e-107">Zie Snel starten: Een app registreren op het [Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) en [Best practices voor het Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0dd5e-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="0dd5e-108">Zie Een [Azure AD-app maken & service principal in de portal - Microsoft-identiteitsplatform voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="0dd5e-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
