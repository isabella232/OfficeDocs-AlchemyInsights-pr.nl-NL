---
title: Problemen met geweigerde toegangs berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051420"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="714c5-102">Problemen met toegang geweigerd berichten in SharePoint/OneDrive Admin Center oplossen</span><span class="sxs-lookup"><span data-stu-id="714c5-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="714c5-103">Als u een bericht toegang geweigerd ontvangt wanneer u probeert te bladeren naar een Admin Center van SharePoint/OneDrive, zorg ervoor dat u [een licentie toewijzen aan de gebruiker](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="714c5-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="714c5-104">Als de gebruiker een licentie heeft, moet u ook ervoor zorgen dat ze [een beheerdersrol](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) die toegang hebben tot de admin Centers worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="714c5-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="714c5-105">Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw gemaakt met de dezelfde UPN (User Principal Name).</span><span class="sxs-lookup"><span data-stu-id="714c5-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="714c5-106">De nieuwe account wordt gemaakt met behulp van een andere waarde van de PUID (paspoort unieke ID).</span><span class="sxs-lookup"><span data-stu-id="714c5-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="714c5-107">Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="714c5-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="714c5-108">Een tweede scenario heeft betrekking op adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OE).</span><span class="sxs-lookup"><span data-stu-id="714c5-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="714c5-109">Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kunnen dit probleem optreden.</span><span class="sxs-lookup"><span data-stu-id="714c5-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="714c5-110">U lost dit probleem, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="714c5-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="714c5-111">Opmerking: als een OneDrive-of SharePoint-Beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.</span><span class="sxs-lookup"><span data-stu-id="714c5-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="714c5-112">[Controleer de servicestatus dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="714c5-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


