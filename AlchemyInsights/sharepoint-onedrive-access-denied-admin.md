---
title: Problemen met geweigerde berichten met toegang oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505374"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="41a63-102">Problemen met geweigerde berichten oplossen in Sharepoint/OneDrive-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="41a63-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="41a63-103">Als u een bericht met geweigerde toegang ontvangt wanneer u probeert naar een Sharepoint/OneDrive-beheercentrum te bladeren, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="41a63-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="41a63-104">Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat aan de gebruiker [een beheerdersrol](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) wordt toegewezen die toegang heeft tot de beheercentra.</span><span class="sxs-lookup"><span data-stu-id="41a63-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="41a63-105">Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde naam van de gebruiker (UPN).</span><span class="sxs-lookup"><span data-stu-id="41a63-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="41a63-106">Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde.</span><span class="sxs-lookup"><span data-stu-id="41a63-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="41a63-107">Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn/haar OneDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="41a63-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="41a63-108">Een tweede scenario omvat adreslijstsynchronisatie met een Organisatie-eenheid (Active Directory organizational unit).</span><span class="sxs-lookup"><span data-stu-id="41a63-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="41a63-109">Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatie worden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.</span><span class="sxs-lookup"><span data-stu-id="41a63-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="41a63-110">Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="41a63-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="41a63-111">Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.</span><span class="sxs-lookup"><span data-stu-id="41a63-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="41a63-112">[Controleer het dashboard servicestatus](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="41a63-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


