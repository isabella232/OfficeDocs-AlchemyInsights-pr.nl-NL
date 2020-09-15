---
title: Delen met externe gebruikers werkt niet
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691570"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="72c66-102">Problemen oplossen met het delen van SharePoint-inhoud met externe gebruikers</span><span class="sxs-lookup"><span data-stu-id="72c66-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="72c66-103">Zorg ervoor dat extern delen is ingeschakeld voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="72c66-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="72c66-104">Ga naar de [ &amp; pagina invoegtoepassingen voor services in het microsoft 365-Beheercentrum](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)en klik op **sites**.</span><span class="sxs-lookup"><span data-stu-id="72c66-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="72c66-105">Zorg dat de instelling is ingeschakeld op aan.</span><span class="sxs-lookup"><span data-stu-id="72c66-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="72c66-106">Als ' alleen bestaande externe gebruikers ' is geselecteerd, controleert u of de externe gebruiker wordt weergegeven in het Microsoft 365-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="72c66-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="72c66-107">Zorg ervoor dat extern delen is ingeschakeld voor de site.</span><span class="sxs-lookup"><span data-stu-id="72c66-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="72c66-108">Voor een klassieke siteverzameling:</span><span class="sxs-lookup"><span data-stu-id="72c66-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="72c66-109">Klik in het nieuwe SharePoint-Beheercentrum in het linkerdeelvenster op **sites**.</span><span class="sxs-lookup"><span data-stu-id="72c66-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="72c66-110">Selecteer de site of sites en klik op het lint op **delen**.</span><span class="sxs-lookup"><span data-stu-id="72c66-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="72c66-111">Voor een team site die hoort bij een Microsoft 365-groep, of een communicatiesite:</span><span class="sxs-lookup"><span data-stu-id="72c66-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="72c66-112">Deze nieuwe site typen hebben dezelfde instelling voordelen als de instelling voor de gehele organisatie, tenzij de instelling voor hele organisatie het delen van bestanden toestaat met behulp van koppelingen waarvoor aanmelding niet is vereist.</span><span class="sxs-lookup"><span data-stu-id="72c66-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="72c66-113">In dit geval kunnen de sites delen delen met nieuwe en bestaande externe gebruikers die zich aanmelden.</span><span class="sxs-lookup"><span data-stu-id="72c66-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="72c66-114">Gebruik het nieuwe SharePoint-Beheercentrum of PowerShell om de instelling voor specifieke sites te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="72c66-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="72c66-115">[Meer informatie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="72c66-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="72c66-116">De instelling voor extern delen voor een site kan meer beperkingen zijn dan de instelling voor de gehele organisatie, maar niet meer beperkt dan de instelling voor de gehele organisatie.</span><span class="sxs-lookup"><span data-stu-id="72c66-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

