---
title: Alleen-lezen voor onderhouds bericht bij een poging om SharePoint of OneDrive te gebruiken
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051276"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="b906d-102">Alleen-lezen voor onderhouds bericht bij een poging om SharePoint of OneDrive te gebruiken</span><span class="sxs-lookup"><span data-stu-id="b906d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="b906d-103">Gebruikers kunnen een **alleen-lezen voor onderhouds** bericht ontvangen wanneer u probeert te gebruiken van SharePoint of OneDrive voor een van de volgende scenario's.</span><span class="sxs-lookup"><span data-stu-id="b906d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="b906d-104">Een geplande of actieve onderhoudsactiviteit.</span><span class="sxs-lookup"><span data-stu-id="b906d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="b906d-105">Controleer ze door naar het [berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter)te navigeren.</span><span class="sxs-lookup"><span data-stu-id="b906d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="b906d-106">Een actief service incident met hoge prioriteit dat kan optreden.</span><span class="sxs-lookup"><span data-stu-id="b906d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="b906d-107">Controleer op eventuele adviezen/incidenten door te navigeren naar de [service status](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b906d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="b906d-108">Een kleine auto-Healing herstelscenario dat kan gebeuren als gevolg van onverwachte gebeurtenissen op de servers die kunnen duren voor minder dan 30 min of zo.</span><span class="sxs-lookup"><span data-stu-id="b906d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="b906d-109">Er zijn geen berichtencentrum of service Health Posts voor deze kleine terugvorderingen, maar je moet heel snel terug naar normaal.</span><span class="sxs-lookup"><span data-stu-id="b906d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="b906d-110">Bij zeer weinig gelegenheden hebben we geconstateerd dat een van de drie hierboven genoemde scenario's de oorzaak zijn geweest, en de service is hersteld, maar de gebruikers browser cache is niet gewist.</span><span class="sxs-lookup"><span data-stu-id="b906d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="b906d-111">Probeer de browser cache te wissen voordat u naar de site navigeert.</span><span class="sxs-lookup"><span data-stu-id="b906d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="b906d-112">Selecteer in de Microsoft Edge-browser **instellingen**en selecteer vervolgens **Privacy en beveiliging**.</span><span class="sxs-lookup"><span data-stu-id="b906d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="b906d-113">Selecteer onder **wissen browsen** **de optie kiezen wat u wilt wissen**.</span><span class="sxs-lookup"><span data-stu-id="b906d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="b906d-114">Selecteer **cookies en opgeslagen website gegevens**en selecteer **Wis**.</span><span class="sxs-lookup"><span data-stu-id="b906d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="b906d-115">Deze stappen kunnen afwijken bij het gebruik van andere browsers zoals Mozilla Firefox of Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="b906d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="b906d-116">Een andere optie is om uw SharePoint-site of OneDrive te openen in een nieuw InPrivate-venster.</span><span class="sxs-lookup"><span data-stu-id="b906d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>