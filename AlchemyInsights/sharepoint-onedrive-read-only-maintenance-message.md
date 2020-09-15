---
title: Alleen-lezen voor onderhouds bericht bij het gebruik van SharePoint of OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670827"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="b544f-102">Alleen-lezen voor onderhouds bericht bij het gebruik van SharePoint of OneDrive</span><span class="sxs-lookup"><span data-stu-id="b544f-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="b544f-103">Gebruikers kunnen een **alleen-lezen bericht ontvangen voor onderhoud** wanneer ze probeert SharePoint of OneDrive te gebruiken voor één van de volgende scenario's.</span><span class="sxs-lookup"><span data-stu-id="b544f-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="b544f-104">Een geplande of actieve onderhouds activiteit.</span><span class="sxs-lookup"><span data-stu-id="b544f-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="b544f-105">Ga naar het [berichtencentrum](https://portal.office.com/adminportal/home#/messagecenter)om dit te controleren.</span><span class="sxs-lookup"><span data-stu-id="b544f-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="b544f-106">Een hoge prioriteit, een actief service voorval dat mogelijk wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="b544f-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="b544f-107">Kijk op een of meer adviseurs/incidenten door naar [service status](https://portal.office.com/adminportal/home#/servicehealth)te navigeren.</span><span class="sxs-lookup"><span data-stu-id="b544f-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="b544f-108">Een klein herstelscenario met automatisch herstel dat kan optreden vanwege eventuele onverwachte gebeurtenissen op de servers die voor minder dan 30 minuten duren.</span><span class="sxs-lookup"><span data-stu-id="b544f-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="b544f-109">Er zijn geen berichtencentrum of service statusberichten voor deze kleine herdetecties, maar u moet altijd weer normaal zijn.</span><span class="sxs-lookup"><span data-stu-id="b544f-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="b544f-110">In slechts een paar gevallen hebben we vastgesteld dat een van de drie scenario's hierboven de oorzaak was en de service hersteld is, maar de browsercache van de gebruikers niet is gewist.</span><span class="sxs-lookup"><span data-stu-id="b544f-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="b544f-111">Probeer de cache van de browser te wissen voordat u naar de site navigeert.</span><span class="sxs-lookup"><span data-stu-id="b544f-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="b544f-112">Selecteer in de browser Microsoft Edge **instellingen**en selecteer vervolgens **Privacy en beveiliging**.</span><span class="sxs-lookup"><span data-stu-id="b544f-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="b544f-113">Selecteer onder **Browse wissen**de **optie Selecteer wat u wilt wissen**.</span><span class="sxs-lookup"><span data-stu-id="b544f-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="b544f-114">Selecteer **cookies en opgeslagen websitegegevens**en selecteer **wissen**.</span><span class="sxs-lookup"><span data-stu-id="b544f-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="b544f-115">Deze stappen kunnen verschillen wanneer u andere browsers gebruikt, zoals Mozilla Firefox of Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="b544f-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="b544f-116">Een andere mogelijkheid is om uw SharePoint-site of OneDrive te openen in een nieuw InPrivate-venster.</span><span class="sxs-lookup"><span data-stu-id="b544f-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>