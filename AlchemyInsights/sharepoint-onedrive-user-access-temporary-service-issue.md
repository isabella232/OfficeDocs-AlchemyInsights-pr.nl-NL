---
title: Prestatieproblemen-SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771239"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="6c41e-102">SharePoint of OneDrive traag, niet beschikbaar of niet beschikbaar voor meerdere gebruikers</span><span class="sxs-lookup"><span data-stu-id="6c41e-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="6c41e-103">Als een OneDrive-of SharePoint-site niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een probleem met een tijdelijke service.</span><span class="sxs-lookup"><span data-stu-id="6c41e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="6c41e-104">[Controleer het dashboard servicestatus](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6c41e-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="6c41e-105">**De gebruiker toevoegen en een licentie verlenen**</span><span class="sxs-lookup"><span data-stu-id="6c41e-105">**Add and license the user**</span></span>

<span data-ttu-id="6c41e-106">Zorg ervoor dat u [licenties toewijst aan gebruikers in Microsoft 365 voor bedrijven](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="6c41e-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="6c41e-107">**Machtigingen toewijzen**</span><span class="sxs-lookup"><span data-stu-id="6c41e-107">**Assign Permissions**</span></span>

<span data-ttu-id="6c41e-108">Als aan de gebruiker een SharePoint-licentie is toegewezen en er nog steeds een bericht toegang geweigerd wordt ontvangen, moet u ervoor zorgen dat het [juiste machtigingsniveau](https://docs.microsoft.com/sharepoint/understanding-permission-levels) is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="6c41e-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="6c41e-109">**Het gebruik van de functie voor toegangsaanvragen overwegen**</span><span class="sxs-lookup"><span data-stu-id="6c41e-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="6c41e-110">Met de [functie voor toegangsaanvragen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kunnen gebruikers toegang aanvragen voor inhoud die hij/zij momenteel niet mag zien.</span><span class="sxs-lookup"><span data-stu-id="6c41e-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="6c41e-111">**Toestaan dat aangepaste scripts toegang hebben tot geweigerde problemen**</span><span class="sxs-lookup"><span data-stu-id="6c41e-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="6c41e-112">Er zijn bepaalde situaties waarin de functie *aangepast script toestaan* een toegang kan presenteren.</span><span class="sxs-lookup"><span data-stu-id="6c41e-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="6c41e-113">Voor een lijst met de desbetreffende functies en de mogelijkheid om de functie uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="6c41e-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="6c41e-114">Ga naar [aangepaste scripts toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="6c41e-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

