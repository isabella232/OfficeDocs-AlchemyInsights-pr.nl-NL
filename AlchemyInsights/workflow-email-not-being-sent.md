---
title: Werkstroome-mail wordt niet verzonden
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766128"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="e9f1b-102">Werkstroome-mail wordt niet verzonden voor een SharePoint-lijst of -bibliotheek</span><span class="sxs-lookup"><span data-stu-id="e9f1b-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="e9f1b-103">E-mail van werkstromen wordt niet naar alle gebruikers of alleen specifieke gebruikers verzonden of u ziet de fout **Het e-mailbericht kan niet worden verzonden. Controleer of de e-mail een geldige ontvanger heeft.**</span><span class="sxs-lookup"><span data-stu-id="e9f1b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="e9f1b-104">Controleer of de gebruiker bestaat in de groep Machtigingen **voor alle personen** (lijst met gebruikersgegevens) voor die siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e9f1b-105">Voorbeeld directe URL:<tenant><sitename>https:// .sharepoint.com/sites/ /_layouts/15/people.aspx? LidmaatschapGroupId=0</span><span class="sxs-lookup"><span data-stu-id="e9f1b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="e9f1b-106">Als de gebruiker niet bestaat, controleert u of de gebruiker is aangemeld bij de pagina.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="e9f1b-107">Als het een externe gebruiker is, moet u ervoor zorgen dat de uitnodiging is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="e9f1b-108">Als de gebruiker wel in de groep machtigingen aanwezig is, controleert u of het e-mailadres juist is.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="e9f1b-109">Als het e-mailadres van de gebruikers hier niet is ingesteld, maakt u een voorbeeldwaarschuwing voor die gebruiker die de synchronisatie van dat gebruikersaccount van gebruikersprofielen van SharePoint naar deze siteverzameling dwingt.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e9f1b-110">E-mail van werkstromen wordt verzonden naar de beheerders van de siteverzameling, maar niet naar andere gebruikers en zie de fout **HTTP Verboden naar <span>https:</span>/URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="e9f1b-111">Zie [Toegang geweigerd wanneer u een e-mail verzendt naar een SharePoint-groep](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="e9f1b-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="e9f1b-112">Controleer ook of de **siteverzamelingsfunctie** voor beperkte toegang voor gebruikersmachtigingen niet actief is.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="e9f1b-113">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="e9f1b-113">Related topics</span></span>
<span data-ttu-id="e9f1b-114">Wilt u Microsoft Flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e9f1b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e9f1b-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="e9f1b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e9f1b-116">SharePoint en Flow</span><span class="sxs-lookup"><span data-stu-id="e9f1b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


