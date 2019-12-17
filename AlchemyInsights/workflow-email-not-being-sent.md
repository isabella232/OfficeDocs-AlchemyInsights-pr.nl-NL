---
title: Werkstroom-e-mail wordt niet verzonden
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049368"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="418dd-102">Werkstroom-e-mail wordt niet verzonden voor een SharePoint-lijst of-bibliotheek</span><span class="sxs-lookup"><span data-stu-id="418dd-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="418dd-103">E-mail van werkstromen wordt niet verzonden naar alle gebruikers of alleen specifieke gebruikers, of u ziet de fout **die het e-mail bericht kan niet worden verzonden. Zorg ervoor dat het e-mail bericht een geldige geadresseerde heeft**.</span><span class="sxs-lookup"><span data-stu-id="418dd-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="418dd-104">Controleer of de gebruiker bestaat in de groep **alle personen** machtigingen (lijst met gebruikersgegevens) voor die siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="418dd-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="418dd-105">Voorbeeld van directe URL<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="418dd-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="418dd-106">Als de gebruiker niet bestaat, controleert u of de gebruiker is aangemeld bij de pagina.</span><span class="sxs-lookup"><span data-stu-id="418dd-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="418dd-107">Als het een externe gebruiker is, controleert u of de uitnodiging is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="418dd-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="418dd-108">Als de gebruiker in de groep machtigingen bestaat, controleert u of het e-mailadres juist is.</span><span class="sxs-lookup"><span data-stu-id="418dd-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="418dd-109">Als het e-mailadres van gebruikers hier niet is ingesteld, maakt u een voorbeeld waarschuwing voor die gebruiker die de synchronisatie van dat gebruikersaccount van gebruikersprofielen van SharePoint naar deze siteverzameling dwingt.</span><span class="sxs-lookup"><span data-stu-id="418dd-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="418dd-110">E-mail van workflows worden verzonden naar de beheerders van de siteverzameling, maar niet naar andere gebruikers en zien de fout **http verboden <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="418dd-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="418dd-111">Zie [toegang geweigerd wanneer u een e-mail bericht naar een SharePoint-groep verzendt](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="418dd-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="418dd-112">Controleer ook of de site verzamelings functie voor **beperkte toegang tot de vergrendelingsmodus van gebruikers** niet actief is.</span><span class="sxs-lookup"><span data-stu-id="418dd-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="418dd-113">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="418dd-113">Related topics</span></span>
<span data-ttu-id="418dd-114">Wilt u Microsoft flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="418dd-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="418dd-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="418dd-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="418dd-116">SharePoint en flow</span><span class="sxs-lookup"><span data-stu-id="418dd-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


