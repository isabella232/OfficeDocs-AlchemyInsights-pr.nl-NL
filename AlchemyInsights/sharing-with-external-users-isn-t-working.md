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
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582770"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="f1eb6-102">Problemen oplossen bij het delen van SharePoint-inhoud met externe gebruikers</span><span class="sxs-lookup"><span data-stu-id="f1eb6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="f1eb6-103">Controleer of extern delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="f1eb6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="f1eb6-104">Ga naar de [ &amp; pagina Services-invoegtoepassingen in het Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **Sites**.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="f1eb6-105">Controleer of de instelling is ingeschakeld om 'Aan' te zetten.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="f1eb6-106">Als 'Alleen bestaande externe gebruikers' zijn geselecteerd, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="f1eb6-107">Zorg ervoor dat extern delen is ingeschakeld voor de site.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="f1eb6-108">Voor een klassieke site collectie:</span><span class="sxs-lookup"><span data-stu-id="f1eb6-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="f1eb6-109">Klik in het nieuwe SharePoint-beheercentrum in het linkerdeelvenster op **sites**.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="f1eb6-110">Selecteer de site of sites en klik op het lint op **Delen**.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="f1eb6-111">Voor een teamsite die deel uitmaakt van een Microsoft 365-groep of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="f1eb6-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="f1eb6-112">Deze nieuwe sitetypen hebben dezelfde instelling voor delen als de instelling voor hele organisatie, tenzij de instelling voor de hele organisatie het delen van bestanden toestaat met koppelingen waarvoor u zich niet hoeft aan te melden.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="f1eb6-113">In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="f1eb6-114">Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-beheercentrum of PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="f1eb6-115">[Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="f1eb6-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f1eb6-116">De instelling voor extern delen voor elke site kan restrictiever zijn dan uw instellingsbrede instelling voor de hele organisatie, maar niet toleranter dan de instelling voor de hele organisatie.</span><span class="sxs-lookup"><span data-stu-id="f1eb6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

