---
title: Dynamics 365 - verkeerde Dashboard toont in Dynamics 365 eenduidige Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747359"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="2c4de-102">Verkeerde dashboard toont in Dynamics 365 eenduidige interface</span><span class="sxs-lookup"><span data-stu-id="2c4de-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="2c4de-103">Er zijn verschillende redenen waarom ziet u mogelijk een ander dashboard dan die u zou verwachten:</span><span class="sxs-lookup"><span data-stu-id="2c4de-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="2c4de-104">De gebruiker heeft een gebruiker standaarddashboard instellen</span><span class="sxs-lookup"><span data-stu-id="2c4de-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="2c4de-105">Meestal kunt u een gebruiker identificeren standaarddashboard is ingesteld als de knop **Als standaard instellen** niet op de opdrachtbalk dashboard weergegeven.</span><span class="sxs-lookup"><span data-stu-id="2c4de-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="2c4de-106">De gebruiker standaarddashboard overschrijft alle andere standaard dashboards, zelfs als de gebruiker de standaarddashboard niet in de huidige app.</span><span class="sxs-lookup"><span data-stu-id="2c4de-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="2c4de-107">Gebruik de volgende tijdelijke oplossing uitschakelen hun standaarddashboard.</span><span class="sxs-lookup"><span data-stu-id="2c4de-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="2c4de-108">Maak een nieuw persoonlijk dashboard.</span><span class="sxs-lookup"><span data-stu-id="2c4de-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="2c4de-109">Die nieuwe dashboard instellen als de gebruikersstandaard.</span><span class="sxs-lookup"><span data-stu-id="2c4de-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="2c4de-110">Verwijder dit dashboard.</span><span class="sxs-lookup"><span data-stu-id="2c4de-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="2c4de-111">Het dashboard is ingesteld in de sitemap</span><span class="sxs-lookup"><span data-stu-id="2c4de-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="2c4de-112">U hebt een organisatie standaarddashboard ingesteld door het selecteren van een dashboard en 'Als standaard instellen' in het systeem aanpassen te kiezen.</span><span class="sxs-lookup"><span data-stu-id="2c4de-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="2c4de-113">Maar het dashboard is gedefinieerd in de ontwerpfunctie van sitemap voorrang op dit dashboard, als de gebruiker toegang tot het heeft.</span><span class="sxs-lookup"><span data-stu-id="2c4de-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="2c4de-114">Als u wilt dat gebruikers toegang tot de dashboard die u hebt ingesteld als de Organisatiestandaard, kunt u:</span><span class="sxs-lookup"><span data-stu-id="2c4de-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="2c4de-115">Stel dat dashboard in de sitemap</span><span class="sxs-lookup"><span data-stu-id="2c4de-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="2c4de-116">Toegang tot het dashboard van de sitemap is gedefinieerd voor gebruikers verwijderen</span><span class="sxs-lookup"><span data-stu-id="2c4de-116">Remove access to the sitemap defined dashboard for those users</span></span>
