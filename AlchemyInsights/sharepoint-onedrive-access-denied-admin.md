---
title: Berichten voor geweigerde toegang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767656"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="53c06-102">Berichten in de Access-Beheercentrum in SharePoint/OneDrive oplossen</span><span class="sxs-lookup"><span data-stu-id="53c06-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="53c06-103">Als u het bericht toegang geweigerd ontvangt wanneer u naar een SharePoint-Beheercentrum probeert te bladeren, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="53c06-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="53c06-104">Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat [aan de gebruiker een beheerdersrol is toegewezen](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) die toegang heeft tot de beheer centra.</span><span class="sxs-lookup"><span data-stu-id="53c06-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="53c06-105">Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met de UPN (User Principal Name) van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="53c06-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="53c06-106">Het nieuwe account wordt gemaakt met behulp van een andere PUID-waarde (Passport unieke ID).</span><span class="sxs-lookup"><span data-stu-id="53c06-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="53c06-107">Wanneer de gebruiker een siteverzameling of de OneDrive probeert te openen, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="53c06-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="53c06-108">Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53c06-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="53c06-109">Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kan dit probleem zich voordoen.</span><span class="sxs-lookup"><span data-stu-id="53c06-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="53c06-110">U kunt dit probleem oplossen door de oorspronkelijke UPN te herstellen met de stappen in het artikel [een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="53c06-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="53c06-111">Opmerking: als een OneDrive-of SharePoint-Beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.</span><span class="sxs-lookup"><span data-stu-id="53c06-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="53c06-112">[Controleer het dashboard servicestatus](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="53c06-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


