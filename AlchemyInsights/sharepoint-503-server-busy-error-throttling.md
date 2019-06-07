---
title: SharePoint Online beperken
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761254"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="181e6-102">SharePoint Online beperken</span><span class="sxs-lookup"><span data-stu-id="181e6-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="181e6-103">Gebruikers ontvangen een 503-server is bezet fout wanneer u probeert om te navigeren naar de SharePoint- of OneDrive sites.</span><span class="sxs-lookup"><span data-stu-id="181e6-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="181e6-104">Deze fout kan worden veroorzaakt door in de SharePoint-service beperken.</span><span class="sxs-lookup"><span data-stu-id="181e6-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="181e6-105">SharePoint Online maakt gebruik van bandbreedtebeperking onderhouden voor optimale prestaties en betrouwbaarheid van de SharePoint Online-service.</span><span class="sxs-lookup"><span data-stu-id="181e6-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="181e6-106">Bandbreedtebeperking beperkt roept het aantal acties van de gebruiker of gelijktijdige (door script of code) om te voorkomen dat overmatig gebruik van bronnen.</span><span class="sxs-lookup"><span data-stu-id="181e6-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="181e6-107">Als u ophalen vertraagde, 99% van de tijd is het gevolg van aangepaste code.</span><span class="sxs-lookup"><span data-stu-id="181e6-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="181e6-108">Voor meer informatie over het beperken Zie, [beperkt of geblokkeerd in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="181e6-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="181e6-109">Als u denkt dat deze fout niet is gerelateerd aan beperken, kunt u controleren of er actieve onderhoud die plaatsvinden op de huurder door te gaan met het [berichtencentrum](https://portal.office.com/adminportal/home#/MessageCenter)is.</span><span class="sxs-lookup"><span data-stu-id="181e6-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="181e6-110">Controleer tot slot u Ga naar de pagina [Status van de Service](https://portal.office.com/adminportal/home#/servicehealth) om te controleren op eventuele aanbevelingen/incidenten die zich zou kunnen voordoen.</span><span class="sxs-lookup"><span data-stu-id="181e6-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

