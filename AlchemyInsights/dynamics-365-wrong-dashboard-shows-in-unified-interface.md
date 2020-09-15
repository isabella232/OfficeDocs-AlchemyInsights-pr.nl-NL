---
title: Dynamics 365-onjuist dashboard wordt weergegeven in de geïntegreerde interface van Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711270"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="756dc-102">Onjuiste dashboard wordt weergegeven in de geïntegreerde interface van Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="756dc-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="756dc-103">Er zijn verschillende redenen waarom een ander dashboard kan worden weergegeven dan de verwachte versie:</span><span class="sxs-lookup"><span data-stu-id="756dc-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="756dc-104">De gebruiker heeft een standaarddashboard voor een gebruiker ingesteld</span><span class="sxs-lookup"><span data-stu-id="756dc-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="756dc-105">Normaalgesproken kunt u aangeven dat het standaarddashboard van een gebruiker is ingesteld als de knop **als standaard instellen** niet wordt weergegeven op de opdrachtbalk van het dashboard.</span><span class="sxs-lookup"><span data-stu-id="756dc-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="756dc-106">Het standaarddashboard van de gebruiker negeert alle andere standaard dashboards, zelfs als het standaarddashboard van de gebruiker zich niet in de huidige app bevindt.</span><span class="sxs-lookup"><span data-stu-id="756dc-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="756dc-107">Gebruik de volgende tijdelijke oplossing om het standaarddashboard uit te heffen.</span><span class="sxs-lookup"><span data-stu-id="756dc-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="756dc-108">Maak een nieuw, persoonlijk dashboard.</span><span class="sxs-lookup"><span data-stu-id="756dc-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="756dc-109">Stel dat nieuwe dashboard als standaard instellen.</span><span class="sxs-lookup"><span data-stu-id="756dc-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="756dc-110">Verwijder het dashboard.</span><span class="sxs-lookup"><span data-stu-id="756dc-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="756dc-111">Het dashboard is ingesteld op de siteoverzicht</span><span class="sxs-lookup"><span data-stu-id="756dc-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="756dc-112">U hebt mogelijk een standaarddashboard voor de organisatie ingesteld door een dashboard te selecteren en ' als standaard instellen ' in te stellen onder ' het systeem aanpassen '.</span><span class="sxs-lookup"><span data-stu-id="756dc-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="756dc-113">Het dashboard dat in de site van de siteoverzicht is gedefinieerd, heeft voorrang op dit dashboard, als de gebruiker er toegang toe heeft.</span><span class="sxs-lookup"><span data-stu-id="756dc-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="756dc-114">Als u wilt dat gebruikers het dashboard kunnen zien dat u hebt ingesteld als de standaardorganisatie, kunt u het volgende doen:</span><span class="sxs-lookup"><span data-stu-id="756dc-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="756dc-115">Dat Dashboard instellen op de siteoverzicht</span><span class="sxs-lookup"><span data-stu-id="756dc-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="756dc-116">De toegang tot het door de site gedefinieerde dashboard voor deze gebruikers verwijderen</span><span class="sxs-lookup"><span data-stu-id="756dc-116">Remove access to the sitemap defined dashboard for those users</span></span>
