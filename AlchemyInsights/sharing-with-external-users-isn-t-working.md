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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502226"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="36e2e-102">SharePoint-inhoud delen met externe gebruikers problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="36e2e-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="36e2e-103">Zorg ervoor dat externe delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="36e2e-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="36e2e-104">Ga naar de [Services &amp; pagina-ins in het Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), en op **websites**.</span><span class="sxs-lookup"><span data-stu-id="36e2e-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="36e2e-105">Controleer of dat de instelling is ingeschakeld op 'Aan'.</span><span class="sxs-lookup"><span data-stu-id="36e2e-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="36e2e-106">Als 'Alleen bestaande externe gebruikers' is ingeschakeld, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="36e2e-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="36e2e-107">Zorg ervoor dat extern delen die zijn ingeschakeld voor de site.</span><span class="sxs-lookup"><span data-stu-id="36e2e-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="36e2e-108">Voor een klassieke siteverzameling:</span><span class="sxs-lookup"><span data-stu-id="36e2e-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="36e2e-109">Klik in het nieuwe SharePoint admin center, in het linkerdeelvenster op **websites**.</span><span class="sxs-lookup"><span data-stu-id="36e2e-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="36e2e-110">Selecteer de site of sites en op het lint, klik op **delen**.</span><span class="sxs-lookup"><span data-stu-id="36e2e-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="36e2e-111">Voor een teamsite die behoort tot een groep van Office 365, of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="36e2e-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="36e2e-112">Deze nieuwe site typen hebben de dezelfde delen als u als instelling voor de hele organisatie, tenzij u de instelling van de hele organisatie ondersteunt het delen van bestanden via de koppelingen die niet vereisen-in.</span><span class="sxs-lookup"><span data-stu-id="36e2e-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="36e2e-113">In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden.</span><span class="sxs-lookup"><span data-stu-id="36e2e-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="36e2e-114">U wijzigt de instelling voor specifieke sites, moet u de nieuwe SharePoint admin center of PowerShell gebruiken.</span><span class="sxs-lookup"><span data-stu-id="36e2e-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="36e2e-115">[Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="36e2e-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="36e2e-116">De externe delen instellen voor elke site is meer beperkend zijn dan de instelling voor de hele organisatie, maar niet meer dan de instelling voor de hele organisatie strikte.</span><span class="sxs-lookup"><span data-stu-id="36e2e-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

