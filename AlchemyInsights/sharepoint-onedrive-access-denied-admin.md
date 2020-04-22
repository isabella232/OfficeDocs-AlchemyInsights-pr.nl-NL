---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758393"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a317f-102">Problemen met toegang geweigerde berichten oplossen in Sharepoint/OneDrive-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="a317f-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a317f-103">Als u een bericht met toegang geweigerd ontvangt wanneer u probeert te bladeren naar een Sharepoint/OneDrive-beheercentrum, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="a317f-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="a317f-104">Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat deze [een beheerdersrol krijgt](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) toegewezen die toegang heeft tot de beheerderscentra.</span><span class="sxs-lookup"><span data-stu-id="a317f-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="a317f-105">Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde gebruikersnaam (UPN).</span><span class="sxs-lookup"><span data-stu-id="a317f-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a317f-106">Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde.</span><span class="sxs-lookup"><span data-stu-id="a317f-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a317f-107">Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn OfaDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="a317f-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a317f-108">Een tweede scenario omvat adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OU).</span><span class="sxs-lookup"><span data-stu-id="a317f-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a317f-109">Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatieworden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.</span><span class="sxs-lookup"><span data-stu-id="a317f-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a317f-110">Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a317f-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="a317f-111">Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijke serviceprobleem.</span><span class="sxs-lookup"><span data-stu-id="a317f-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a317f-112">[Controleer het dashboard voor servicestatus](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a317f-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


