---
title: Delen met externe gebruikers werkt niet
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502226"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e5ba6-102">Problemen met het delen van SharePoint-inhoud met externe gebruikers oplossen</span><span class="sxs-lookup"><span data-stu-id="e5ba6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e5ba6-103">Zorg ervoor dat extern delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="e5ba6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e5ba6-104">Ga naar de [pagina &amp; Services-invoegtoepassingen in het Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **sites**.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e5ba6-105">Zorg ervoor dat de instelling is ingeschakeld op ' aan '.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e5ba6-106">Als ' alleen bestaande externe gebruikers ' is geselecteerd, controleert u of de externe gebruiker wordt vermeld in het Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e5ba6-107">Zorg ervoor dat extern delen is ingeschakeld voor de site.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e5ba6-108">Voor een klassieke siteverzameling:</span><span class="sxs-lookup"><span data-stu-id="e5ba6-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e5ba6-109">In het nieuwe SharePoint-Beheercentrum, in het linkerdeelvenster, klikt u op **sites**.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e5ba6-110">Selecteer de site of sites en klik op het lint op **delen**.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e5ba6-111">Voor een team site die behoort tot een Office 365-groep of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="e5ba6-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e5ba6-112">Deze nieuwe site typen hebben dezelfde instelling voordelen als de instelling voor de hele organisatie, tenzij de organisatiebrede instelling het delen van bestanden toestaat met behulp van koppelingen die niet hoeven te worden aangemeld.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e5ba6-113">In dit geval kunnen de sites delen met nieuwe en bestaande externe gebruikers die zich aanmelden.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e5ba6-114">Als u de instelling voor specifieke sites wilt wijzigen, gebruikt u het nieuwe SharePoint-Beheercentrum of PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e5ba6-115">[Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e5ba6-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e5ba6-116">De instelling voor extern delen voor elke site kan restrictiever zijn dan de instelling van de hele organisatie, maar niet meer toelaatbaar dan de organisatiebrede instelling.</span><span class="sxs-lookup"><span data-stu-id="e5ba6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

