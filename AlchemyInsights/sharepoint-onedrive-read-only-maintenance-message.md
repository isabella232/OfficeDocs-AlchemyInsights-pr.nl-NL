---
title: Alleen-lezen voor onderhoud wordt weergegeven wanneer u probeert te gebruiken van SharePoint of OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620718"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="3fba2-102">Alleen-lezen voor onderhoud wordt weergegeven wanneer u probeert te gebruiken van SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="3fba2-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="3fba2-103">Gebruikers kunnen een bericht **Alleen-lezen voor onderhoud** tijdens het gebruik van SharePoint of OneDrive voor een van de volgende scenario's.</span><span class="sxs-lookup"><span data-stu-id="3fba2-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="3fba2-104">Een geplande of actieve onderhoudsactiviteiten.</span><span class="sxs-lookup"><span data-stu-id="3fba2-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="3fba2-105">Controleer of ze door te gaan met het [Berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="3fba2-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="3fba2-106">Een hoge prioriteit actieve service incident dat zich zou kunnen voordoen.</span><span class="sxs-lookup"><span data-stu-id="3fba2-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="3fba2-107">Controleren op eventuele aanbevelingen/incidenten door te gaan voor de [Gezondheid van de Service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3fba2-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="3fba2-108">Een kleine automatische retoucheren herstelscenario dat kan gebeuren als gevolg van een onverwachte gebeurtenissen op de servers die voor minder dan 30 minuten of zo mogelijk laatste.</span><span class="sxs-lookup"><span data-stu-id="3fba2-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="3fba2-109">Er zijn geen Message Center of Health Service post voor deze kleine terugvorderingen, maar moet worden zeer binnenkort weer in de normale.</span><span class="sxs-lookup"><span data-stu-id="3fba2-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="3fba2-110">In enkele gevallen waargenomen we dat een van de drie scenario's hierboven vermeld zijn de oorzaak, en service is hersteld, maar de gebruikers browsercache nog niet is gewist van.</span><span class="sxs-lookup"><span data-stu-id="3fba2-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="3fba2-111">Probeer om de cache van de browser wissen voordat u naar de site navigeren.</span><span class="sxs-lookup"><span data-stu-id="3fba2-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="3fba2-112">Selecteer **Instellingen**en selecteer **Privacy en beveiliging**in de browser Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="3fba2-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="3fba2-113">Selecteer onder het **wissen bladeren**, **kiezen wat u wilt wissen**.</span><span class="sxs-lookup"><span data-stu-id="3fba2-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="3fba2-114">Selecteer **Cookies en gegevens opgeslagen websites**en selecteer **wissen**.</span><span class="sxs-lookup"><span data-stu-id="3fba2-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="3fba2-115">Deze stappen kunnen verschillen bij het gebruik van andere browsers zoals Mozilla Firefox of Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="3fba2-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="3fba2-116">Een andere optie zou zijn voor het openen van uw SharePoint-site of OneDrive in een nieuw venster voor InPrivate-navigatie.</span><span class="sxs-lookup"><span data-stu-id="3fba2-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>