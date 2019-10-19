---
title: Dynamics 365-onjuist dashboard wordt weergegeven in Dynamics 365 unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528546"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="77eab-102">Onjuist dashboard wordt weergegeven in Dynamics 365 unified interface</span><span class="sxs-lookup"><span data-stu-id="77eab-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="77eab-103">Er zijn verschillende redenen waarom u een ander Dashboard zien dan het overzicht dat u verwacht:</span><span class="sxs-lookup"><span data-stu-id="77eab-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="77eab-104">De gebruiker heeft een standaarddashboard voor gebruikers ingesteld</span><span class="sxs-lookup"><span data-stu-id="77eab-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="77eab-105">Meestal u een standaarddashboard van de gebruiker instellen als de knop **als standaard instellen** niet wordt weergegeven in de opdrachtbalk van het dashboard.</span><span class="sxs-lookup"><span data-stu-id="77eab-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="77eab-106">Het standaarddashboard van de gebruiker overschrijft alle andere standaard dashboards, zelfs als het standaarddashboard van de gebruiker zich niet in de huidige app bevindt.</span><span class="sxs-lookup"><span data-stu-id="77eab-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="77eab-107">Gebruik de volgende oplossing om het standaarddashboard te ontkoppelen.</span><span class="sxs-lookup"><span data-stu-id="77eab-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="77eab-108">Maak een nieuw persoonlijk dashboard.</span><span class="sxs-lookup"><span data-stu-id="77eab-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="77eab-109">Stel dat nieuwe dashboard als de gebruiker standaard.</span><span class="sxs-lookup"><span data-stu-id="77eab-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="77eab-110">Verwijder dat Dashboard.</span><span class="sxs-lookup"><span data-stu-id="77eab-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="77eab-111">Het dashboard is ingesteld in de sitemap</span><span class="sxs-lookup"><span data-stu-id="77eab-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="77eab-112">Mogelijk hebt u een standaarddashboard van een organisatie ingesteld door een dashboard te selecteren en ' als standaard instellen ' te kiezen onder ' het systeem aanpassen '.</span><span class="sxs-lookup"><span data-stu-id="77eab-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="77eab-113">Maar het dashboard dat is gedefinieerd in de sitemapontwerper heeft voorrang op dit dashboard, als de gebruiker er toegang toe heeft.</span><span class="sxs-lookup"><span data-stu-id="77eab-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="77eab-114">Als u wilt dat gebruikers het dashboard zien dat u hebt ingesteld als de standaardorganisatie, u:</span><span class="sxs-lookup"><span data-stu-id="77eab-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="77eab-115">Dat Dashboard instellen in de sitemap</span><span class="sxs-lookup"><span data-stu-id="77eab-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="77eab-116">Verwijder de toegang tot het door de sitemap gedefinieerde dashboard voor die gebruikers</span><span class="sxs-lookup"><span data-stu-id="77eab-116">Remove access to the sitemap defined dashboard for those users</span></span>
