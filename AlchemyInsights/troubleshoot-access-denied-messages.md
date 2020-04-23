---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759795"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ad9da-102">Problemen met toegang geweigerde berichten oplossen</span><span class="sxs-lookup"><span data-stu-id="ad9da-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ad9da-103">Als iemand een bericht 'Toegang geweigerd' heeft ontvangen in een gedeelde map in SharePoint, heeft de beheerder van de siteverzameling mogelijk de modus 'Beperkte toegang tot toestemming voor gebruikers' ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="ad9da-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ad9da-104">Ga als volgt te werk om dit uit te schakelen:</span><span class="sxs-lookup"><span data-stu-id="ad9da-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ad9da-105">Blader naar de site, klik op het pictogram Instellingen en klik vervolgens op **Site-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="ad9da-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ad9da-106">Klik **onder Beheer van siteverzameling**op Onderdelen voor **siteverzameling**.</span><span class="sxs-lookup"><span data-stu-id="ad9da-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ad9da-107">Klik naast de modus Voor het **vergrendelen van gebruikersmachtigingen**met beperkte toegang op **Deactiveren**.</span><span class="sxs-lookup"><span data-stu-id="ad9da-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ad9da-108">Een bericht Met toegang geweigerd kan ook optreden voor gedeelde mappen als de site een publicerende site is.</span><span class="sxs-lookup"><span data-stu-id="ad9da-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ad9da-109">Zie Toegang [geweigerd bij het openen van een gedeelde map](https://go.microsoft.com/fwlink/?linkid=2004317)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="ad9da-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ad9da-110">Als iemand een bericht 'Toegang geweigerd' heeft gekregen wanneer hij toegangsverzoeken probeert te bekijken, moet de gebruiker worden toegevoegd als beheerder van de siteverzameling of als lid van de groep Eigenaren voor de site.</span><span class="sxs-lookup"><span data-stu-id="ad9da-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ad9da-111">Zie [lijst Toegang tot geweigerde toegang tot toegangsverzoeken](https://go.microsoft.com/fwlink/?linkid=2004220)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="ad9da-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ad9da-112">Zie [Access Denied wanneer een gebruikersaccount is gesynchroniseerd met Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)als een gebruiker een bericht 'Toegang geweigerd' heeft gekregen nadat deze is verwijderd uit Active Directory on-premises en vervolgens is toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="ad9da-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

