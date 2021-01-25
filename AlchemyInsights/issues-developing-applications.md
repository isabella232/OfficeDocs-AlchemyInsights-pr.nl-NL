---
title: Problemen met het ontwikkelen van toepassingen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974305"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="3926c-102">Problemen met het ontwikkelen van toepassingen</span><span class="sxs-lookup"><span data-stu-id="3926c-102">Issues developing applications</span></span>

<span data-ttu-id="3926c-103">Zie de volgende artikelen voor informatie over het oplossen van veelvoorkomende problemen bij het maken van Azure Active Directory (AD)-apps:</span><span class="sxs-lookup"><span data-stu-id="3926c-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="3926c-104">Ik zie problemen met aanmelden bij toepassing (en) met alleen de Chrome-browser</span><span class="sxs-lookup"><span data-stu-id="3926c-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="3926c-105">Ik weet niet hoe ik de standaardwaarden van de token levensduur voor mijn toepassing Wijzig</span><span class="sxs-lookup"><span data-stu-id="3926c-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="3926c-106">Ik weet niet hoe de instemming van de toepassing werkt</span><span class="sxs-lookup"><span data-stu-id="3926c-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="3926c-107">Ik weet niet hoe ik machtigingen voor de toepassing moet verlenen</span><span class="sxs-lookup"><span data-stu-id="3926c-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="3926c-108">Ik weet het verschil tussen gedelegeerde en Toepassingsmachtigingen niet</span><span class="sxs-lookup"><span data-stu-id="3926c-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="3926c-109">\***Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (Aad-grafiek)** _</span><span class="sxs-lookup"><span data-stu-id="3926c-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="3926c-110">Vanaf 30 juni 2020 worden niet langer nieuwe functies toegevoegd aan Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD-grafiek).</span><span class="sxs-lookup"><span data-stu-id="3926c-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="3926c-111">We bieden technische ondersteuning en beveiligingsupdates, maar bieden geen functie-updates meer.</span><span class="sxs-lookup"><span data-stu-id="3926c-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="3926c-112">Vanaf 30 juni 2022 wordt de ondersteuning voor ADAL en AAD-grafiek beëindigd en ontvangt u niet langer technische ondersteuning en beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="3926c-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="3926c-113">Als gevolg van deze voorwaarde zijn de consequenties het volgende:</span><span class="sxs-lookup"><span data-stu-id="3926c-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="3926c-114">Apps die gebruikmaken van ADAL op bestaande versie van het besturingssysteem werken na dit moment nog niet, maar krijgen geen technische ondersteuning of beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="3926c-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="3926c-115">Apps die gebruikmaken van AAD-grafiek na deze periode, kunnen mogelijk niet langer antwoorden ontvangen van het eindpunt van een AAD-grafiek</span><span class="sxs-lookup"><span data-stu-id="3926c-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="3926c-116">_ *ADAL-migratie*\*</span><span class="sxs-lookup"><span data-stu-id="3926c-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="3926c-117">Als u Microsoft apps gebruikt, raden we u aan een update uit te voeren voor de Microsoft Authentication Library (MSAL), met de meest recente functies en beveiligingsupdates.</span><span class="sxs-lookup"><span data-stu-id="3926c-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="3926c-118">Deze aanbevelingen bevindt zich in de context van Microsoft die het proces voor het migreren van de apps naar MSAL door de einde datum van de ondersteuning te bieden.</span><span class="sxs-lookup"><span data-stu-id="3926c-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="3926c-119">De migratie door Microsoft van zijn apps naar MSAL garandeert dat de apps gebruikmaken van de voortdurende beveiliging en functieverbeteringen van MSAL.</span><span class="sxs-lookup"><span data-stu-id="3926c-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="3926c-120">Lees de veelgestelde vragen over ADAL</span><span class="sxs-lookup"><span data-stu-id="3926c-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="3926c-121">Meer informatie over hoe u apps migreert op een platform basis</span><span class="sxs-lookup"><span data-stu-id="3926c-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="3926c-122">Als u hulp nodig hebt bij het begrijpen van de apps van ADAL, raden we u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers (Isv's) of app-providers.</span><span class="sxs-lookup"><span data-stu-id="3926c-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="3926c-123">Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw Tenant bieden.</span><span class="sxs-lookup"><span data-stu-id="3926c-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="3926c-124">**Migratie van AAD-grafieken**</span><span class="sxs-lookup"><span data-stu-id="3926c-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="3926c-125">Voor toepassingen die gebruikmaken van AAD Graph, volgt u onze richtlijnen voor het migreren van AAD-grafiek-apps naar Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="3926c-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="3926c-126">[Onze migratie controlelijst biedt een aantekening aan de slag](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="3926c-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="3926c-127">De registratie portal van Azure app toont welke toepassingen gebruikmaken van een AAD-grafiek.</span><span class="sxs-lookup"><span data-stu-id="3926c-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="3926c-128">We raden u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met onafhankelijke softwareleveranciers (Isv's) of app-providers.</span><span class="sxs-lookup"><span data-stu-id="3926c-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="3926c-129">Microsoft-ondersteuning kan u ook informatie geven over het gebruik van AAD-grafieken in uw Tenant.</span><span class="sxs-lookup"><span data-stu-id="3926c-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







