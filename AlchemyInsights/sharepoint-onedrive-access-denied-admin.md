---
title: Problemen oplossen met berichten die de toegang geweigerd
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503522"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="455cd-102">Problemen oplossen met berichten in Sharepoint OneDrive/Admin Center toegang geweigerd</span><span class="sxs-lookup"><span data-stu-id="455cd-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="455cd-103">Als u toegang geweigerd tijdens een poging om te bladeren naar een Sharepoint OneDrive/Admin Center ontvangt, moet u controleren dat u [een licentie voor de gebruiker toewijzen](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="455cd-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="455cd-104">Als de gebruiker een licentie heeft, moet u ervoor dat ze [een rol toegewezen aan](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) die toegang heeft tot de admin-centers.</span><span class="sxs-lookup"><span data-stu-id="455cd-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="455cd-105">Dit probleem kan ook optreden wanneer een gebruiker is verwijderd en opnieuw met de dezelfde UPN (User Principal Name gemaakt).</span><span class="sxs-lookup"><span data-stu-id="455cd-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="455cd-106">De nieuwe account is gemaakt met behulp van een andere waarde voor de PUID (unieke Passport-ID).</span><span class="sxs-lookup"><span data-stu-id="455cd-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="455cd-107">Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuist PUID.</span><span class="sxs-lookup"><span data-stu-id="455cd-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="455cd-108">Een tweede scenario heeft betrekking op directory synchronisatie met een organisatie-eenheid (OU) van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="455cd-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="455cd-109">Als gebruikers hebben al aangemeld bij SharePoint, worden verplaatst naar een andere organisatie-eenheid en resynced met SharePoint, kunnen zij dit probleem optreden.</span><span class="sxs-lookup"><span data-stu-id="455cd-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="455cd-110">Dit probleem op te lossen moet u weer de oorspronkelijke UPN met de stappen in het artikel, het [herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="455cd-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="455cd-111">Opmerking: Als een OneDrive of SharePoint Admin center niet beschikbaar voor meerdere gebruikers die eerder toegang had is, kan er een tijdelijke service-probleem.</span><span class="sxs-lookup"><span data-stu-id="455cd-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="455cd-112">[Controleer de gezondheid servicedashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="455cd-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


