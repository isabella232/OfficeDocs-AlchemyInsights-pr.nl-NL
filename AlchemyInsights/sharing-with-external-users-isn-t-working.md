---
title: Delen met externe gebruikers werkt niet
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767244"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="f65be-102">Problemen oplossen bij het delen van SharePoint-inhoud met externe gebruikers</span><span class="sxs-lookup"><span data-stu-id="f65be-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="f65be-103">Controleer of extern delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="f65be-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="f65be-104">Ga naar de [pagina Invoegtoepassing &amp; Services in het Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **Sites**.</span><span class="sxs-lookup"><span data-stu-id="f65be-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="f65be-105">Controleer of de instelling is ingeschakeld in 'Aan'.</span><span class="sxs-lookup"><span data-stu-id="f65be-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="f65be-106">Als 'Alleen bestaande externe gebruikers' is geselecteerd, controleert u of de externe gebruiker wordt vermeld in het Microsoft 365-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="f65be-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="f65be-107">Zorg ervoor dat extern delen is ingeschakeld voor de site.</span><span class="sxs-lookup"><span data-stu-id="f65be-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="f65be-108">Voor een klassieke site collectie:</span><span class="sxs-lookup"><span data-stu-id="f65be-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="f65be-109">Klik in het nieuwe SharePoint-beheercentrum in het linkerdeelvenster op **sites**.</span><span class="sxs-lookup"><span data-stu-id="f65be-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="f65be-110">Selecteer de site of sites en klik op het lint op **Delen**.</span><span class="sxs-lookup"><span data-stu-id="f65be-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="f65be-111">Voor een teamsite die deel uitmaakt van een Office 365-groep of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="f65be-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="f65be-112">Deze nieuwe sitetypen hebben dezelfde instelling voor delen als de instelling voor uw hele organisatie, tenzij de instelling voor de hele organisatie het delen van bestanden toestaat met koppelingen waarvoor geen aanmelding vereist is.</span><span class="sxs-lookup"><span data-stu-id="f65be-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="f65be-113">In dit geval staan de sites het delen toe met nieuwe en bestaande externe gebruikers die zich aanmelden.</span><span class="sxs-lookup"><span data-stu-id="f65be-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="f65be-114">Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-beheercentrum of PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f65be-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="f65be-115">[Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="f65be-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f65be-116">De instelling voor extern delen voor elke site kan restrictiever zijn dan uw organisatiebrede instelling, maar niet toleranter dan de organisatiebrede instelling.</span><span class="sxs-lookup"><span data-stu-id="f65be-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

