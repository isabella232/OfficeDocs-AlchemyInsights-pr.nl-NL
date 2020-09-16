---
title: E-mail van werkstroom wordt niet verzonden
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748984"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="7d097-102">E-mail van werkstroom wordt niet verzonden voor een SharePoint-lijst of-bibliotheek</span><span class="sxs-lookup"><span data-stu-id="7d097-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="7d097-103">E-mail van werkstromen wordt niet naar alle gebruikers of alleen specifieke gebruikers verzonden of u ziet de fout **het e-mailbericht kan niet worden verzonden. Zorg ervoor dat het e-mailbericht een geldige geadresseerde heeft**.</span><span class="sxs-lookup"><span data-stu-id="7d097-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="7d097-104">Controleer of de gebruiker in de groep machtigingen voor **alle personen** (gebruikersgegevens) voor die siteverzameling is opgenomen.</span><span class="sxs-lookup"><span data-stu-id="7d097-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="7d097-105">Voorbeeld van directe URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="7d097-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="7d097-106">Als de gebruiker niet bestaat, moet u ervoor zorgen dat de gebruiker is aangemeld bij de pagina.</span><span class="sxs-lookup"><span data-stu-id="7d097-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="7d097-107">Als het om een externe gebruiker gaat, controleert u of de uitnodiging is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="7d097-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="7d097-108">Als de gebruiker in de groep machtigingen bestaat, controleert u of het e-mailadres juist is.</span><span class="sxs-lookup"><span data-stu-id="7d097-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="7d097-109">Als het e-mailadres van gebruikers hier niet is ingesteld, maakt u een voorbeeld waarschuwing voor de gebruiker, die de synchronisatie van die gebruikersaccount van gebruikersprofielen van SharePoint tot deze siteverzameling afdwingt.</span><span class="sxs-lookup"><span data-stu-id="7d097-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="7d097-110">E-mail van werkstromen wordt verzonden naar de beheerders van siteverzamelingen, maar niet naar andere gebruikers en zie de fout **http niet toegestaan voor <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="7d097-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="7d097-111">Zie [toegang geweigerd wanneer u een e-mailbericht naar een SharePoint-groep verzendt](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="7d097-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="7d097-112">Zorg er ook voor dat de functie voor het **vergrendelen van gebruikersmachtigingen voor gebruikers met beperkte toegang** niet is geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="7d097-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="7d097-113">Verwante onderwerpen</span><span class="sxs-lookup"><span data-stu-id="7d097-113">Related topics</span></span>
<span data-ttu-id="7d097-114">Wilt u Microsoft flow uitproberen in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="7d097-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7d097-115">Stroom maken</span><span class="sxs-lookup"><span data-stu-id="7d097-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7d097-116">SharePoint en flow</span><span class="sxs-lookup"><span data-stu-id="7d097-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


