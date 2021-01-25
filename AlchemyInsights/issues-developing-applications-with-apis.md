---
title: Problemen met het ontwikkelen van toepassingen met Api's
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
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974380"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="058d1-102">Problemen met het ontwikkelen van toepassingen met Api's</span><span class="sxs-lookup"><span data-stu-id="058d1-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="058d1-103">Als u wilt beginnen met de API van Azure Active Directory Graph, raadpleegt u de [introductiehandleiding voor Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) of raadpleegt u de documentatie over de [interactieve Azure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="058d1-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="058d1-104">**Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD-grafiek)**</span><span class="sxs-lookup"><span data-stu-id="058d1-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="058d1-105">**Vanaf 30 juni 2020** worden niet langer nieuwe functies toegevoegd aan ADAL en Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="058d1-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="058d1-106">We bieden technische ondersteuning en beveiligingsupdates, maar bieden geen functie-updates meer.</span><span class="sxs-lookup"><span data-stu-id="058d1-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="058d1-107">**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigd en zal u niet langer technische ondersteuning en beveiligingsupdates bieden.</span><span class="sxs-lookup"><span data-stu-id="058d1-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="058d1-108">Apps die gebruikmaken van ADAL op bestaande versie van het besturingssysteem werken na dit moment nog niet, maar krijgen geen technische ondersteuning of beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="058d1-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="058d1-109">Apps die gebruikmaken van Azure AD Graph na dit tijdstip, kunnen mogelijk geen antwoorden meer ontvangen van het Azure AD-eindpunt.</span><span class="sxs-lookup"><span data-stu-id="058d1-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="058d1-110">**ADAL-migratie**</span><span class="sxs-lookup"><span data-stu-id="058d1-110">**ADAL Migration**</span></span>

<span data-ttu-id="058d1-111">We raden u aan een update uit te voeren voor de [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), met de meest recente functies en beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="058d1-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="058d1-112">Als u Microsoft-apps gebruikt, moet u weten dat Microsoft de toepassing van de einde-ondersteunings deadline zal gebruiken voor het migreren van de toepassingen en om te zorgen dat ze profiteren van de voortdurende beveiliging en functieverbeteringen van MSAL.</span><span class="sxs-lookup"><span data-stu-id="058d1-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="058d1-113">[Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="058d1-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="058d1-114">[Meer informatie over hoe u apps migreert op een platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="058d1-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="058d1-115">Als u meer informatie wilt over het gebruik van ADAL, raden we u aan alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met Isv's of app-providers.</span><span class="sxs-lookup"><span data-stu-id="058d1-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="058d1-116">Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw Tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="058d1-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="058d1-117">**Migratie van AAD-grafieken**</span><span class="sxs-lookup"><span data-stu-id="058d1-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="058d1-118">Volg voor toepassingen die gebruikmaken van Azure AD Graph onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="058d1-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="058d1-119">[Onze migratie controlelijst biedt een aantekening aan de slag](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="058d1-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="058d1-120">De registratie portal van Azure app toont welke toepassingen gebruikmaken van een AAD-grafiek.</span><span class="sxs-lookup"><span data-stu-id="058d1-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="058d1-121">We raden u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met Isv's of app-providers.</span><span class="sxs-lookup"><span data-stu-id="058d1-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="058d1-122">Microsoft-ondersteuning kan u ook een lijst met alle AAD-grafiek gebruik in uw Tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="058d1-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="058d1-123">Als u wilt dat de app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of de beheerder deze de juiste machtigingen verlenen via een toestemming procedure.</span><span class="sxs-lookup"><span data-stu-id="058d1-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="058d1-124">De [verwijzing naar machtigingen van Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) bevat de machtigingen die zijn gekoppeld aan elke primaire set Microsoft Graph-api's.</span><span class="sxs-lookup"><span data-stu-id="058d1-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="058d1-125">Ook biedt u informatie over het gebruik van de machtigingen.</span><span class="sxs-lookup"><span data-stu-id="058d1-125">It also provides guidance about how to use the permissions.</span></span>
