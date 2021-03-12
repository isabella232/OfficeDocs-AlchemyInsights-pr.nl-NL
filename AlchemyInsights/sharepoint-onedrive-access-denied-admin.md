---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707949"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ab4a4-102">Problemen met toegang geweigerde berichten in sharepoint/OneDrive-beheercentrum oplossen</span><span class="sxs-lookup"><span data-stu-id="ab4a4-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ab4a4-103">Als u een bericht ontvangt dat de toegang is geweigerd wanneer u naar een Sharepoint/OneDrive-beheercentrum bladert, moet u ervoor zorgen dat u een licentie [toewijst aan de gebruiker.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="ab4a4-104">Als de gebruiker een licentie heeft, moet [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) u er ook voor zorgen dat aan de gebruiker een beheerdersrol is toegewezen die toegang heeft tot de beheercentra.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="ab4a4-105">Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde USER PRINCIPAL Name (UPN).</span><span class="sxs-lookup"><span data-stu-id="ab4a4-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ab4a4-106">Het nieuwe account wordt gemaakt met behulp van een andere waarde voor de PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="ab4a4-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ab4a4-107">Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of oneDrive, beschikt de gebruiker over een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ab4a4-108">Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid (OU) van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ab4a4-109">Als gebruikers zich al hebben aangemeld bij SharePoint, en vervolgens worden verplaatst naar een andere OU en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ervaren.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ab4a4-110">U kunt dit probleem oplossen door de oorspronkelijke UPN te herstellen volgens de stappen in het artikel, Een gebruiker [herstellen in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="ab4a4-111">Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ab4a4-112">[Bekijk het dashboard voor de service status.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


