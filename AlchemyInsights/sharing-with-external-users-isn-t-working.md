---
title: Delen met externe gebruikers werkt niet.
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207680"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="7e93b-102">SharePoint-inhoud delen met externe gebruikers problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="7e93b-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="7e93b-103">Zorg ervoor dat externe delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="7e93b-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="7e93b-104">Ga naar de [Services &amp; pagina-ins in het Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), en op **websites**.</span><span class="sxs-lookup"><span data-stu-id="7e93b-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="7e93b-p101">Controleer of dat de instelling is ingeschakeld op 'Aan'. Als 'Alleen bestaande externe gebruikers' is ingeschakeld, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="7e93b-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="7e93b-p102">Zorg ervoor dat extern delen die zijn ingeschakeld voor de site. Voor een klassieke siteverzameling:</span><span class="sxs-lookup"><span data-stu-id="7e93b-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="7e93b-109">Klik op **siteverzamelingen**in het klassieke SharePoint admin center, in het linkerdeelvenster.</span><span class="sxs-lookup"><span data-stu-id="7e93b-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="7e93b-110">Selecteer de site of sites en op het lint, klik op **delen**.</span><span class="sxs-lookup"><span data-stu-id="7e93b-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="7e93b-111">Voor een teamsite die behoort tot een groep van Office 365, of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="7e93b-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="7e93b-p103">Deze nieuwe site typen hebben de dezelfde delen als u als instelling voor de hele organisatie, tenzij u de instelling van de hele organisatie ondersteunt het delen van bestanden via de koppelingen die niet vereisen-in. In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden. U wijzigt de instelling voor specifieke sites, moet u de nieuwe SharePoint admin center (voorbeeld) of PowerShell gebruiken. [Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="7e93b-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="7e93b-116">De externe delen instellen voor elke site is meer beperkend zijn dan de instelling voor de hele organisatie, maar niet meer dan de instelling voor de hele organisatie strikte.</span><span class="sxs-lookup"><span data-stu-id="7e93b-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

