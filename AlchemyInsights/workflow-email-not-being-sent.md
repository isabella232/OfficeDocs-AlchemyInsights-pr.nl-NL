---
title: Werkstroom e-mailbericht wordt niet verzonden
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530863"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="b0c30-102">Werkstroom e-mailbericht wordt niet verzonden voor een SharePoint-lijst of -bibliotheek</span><span class="sxs-lookup"><span data-stu-id="b0c30-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="b0c30-103">E-mailadres van werkstromen worden niet verzonden naar alle gebruikers of alleen bepaalde gebruikers of ziet u dat de fout **het e-mailbericht kan niet worden verzonden. Controleer of het e-mailbericht heeft een geldige geadresseerde**.</span><span class="sxs-lookup"><span data-stu-id="b0c30-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="b0c30-104">Controleer of de gebruiker in de machtigingsgroep **Alle mensen** (lijst met gebruikersgegevens) voor die siteverzameling bestaat.</span><span class="sxs-lookup"><span data-stu-id="b0c30-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="b0c30-105">Voorbeeld van een directe URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="b0c30-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="b0c30-106">Als de gebruiker niet bestaat, moet u dat de gebruiker is aangemeld op de pagina.</span><span class="sxs-lookup"><span data-stu-id="b0c30-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="b0c30-107">Zorg dat de uitnodiging is geaccepteerd als een externe gebruiker is.</span><span class="sxs-lookup"><span data-stu-id="b0c30-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="b0c30-108">Als de gebruiker in de machtigingsgroep bestaat, moet dat het e-mailadres juist is.</span><span class="sxs-lookup"><span data-stu-id="b0c30-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="b0c30-109">Als de gebruikers e-mailadres hier niet is ingesteld, maakt u een waarschuwing voor een monster voor die gebruiker, waardoor de synchronisatie van die account van gebruikers profielen van SharePoint voor deze siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="b0c30-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="b0c30-110">E-mailadres van werkstromen worden verzonden naar beheerders van de siteverzameling, maar niet voor andere gebruikers en Zie de fout **HTTP verboden <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="b0c30-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="b0c30-111">Zie [De toegang geweigerd wanneer u een e-mail naar een SharePoint-groep sturen](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="b0c30-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="b0c30-112">Controleer ook of de **modus met beperkte toegang gebruiker machtiging lockdown** siteverzamelingfunctie is niet actief.</span><span class="sxs-lookup"><span data-stu-id="b0c30-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="b0c30-113">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="b0c30-113">Related topics</span></span>
<span data-ttu-id="b0c30-114">Wilt u proberen Microsoft Flow in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="b0c30-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b0c30-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="b0c30-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b0c30-116">SharePoint en stroom</span><span class="sxs-lookup"><span data-stu-id="b0c30-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


