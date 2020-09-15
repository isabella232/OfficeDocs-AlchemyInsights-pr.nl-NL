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
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690778"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="5c6bc-102">Berichten voor geweigerde toegang</span><span class="sxs-lookup"><span data-stu-id="5c6bc-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="5c6bc-103">Als iemand het bericht ' toegang geweigerd ' heeft gekregen voor een gedeelde map in SharePoint, heeft de beheerder van de siteverzameling mogelijk de vergrendelingsmodus voor gebruikersmachtigingen met beperkte toegang ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="5c6bc-104">Om dit uit te schakelen:</span><span class="sxs-lookup"><span data-stu-id="5c6bc-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="5c6bc-105">Ga naar de site, klik op het pictogram instellingen en klik vervolgens op **site-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="5c6bc-106">Klik onder beheer van de **siteverzameling**op onderdelen van de **site**verzameling.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="5c6bc-107">Klik naast de **vergrendelingsmodus voor gebruikers met beperkte toegang**op **deactiveren**.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="5c6bc-108">Als de site een publicerende site is, kan het bericht toegang geweigerd ook voor gedeelde mappen plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="5c6bc-109">Zie [toegang geweigerd wanneer u een gedeelde map opent](https://go.microsoft.com/fwlink/?linkid=2004317)voor informatie.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="5c6bc-110">Als iemand het bericht ' toegang geweigerd ' heeft bij het weergeven van toegangsaanvragen, moet de gebruiker worden toegevoegd als een beheerder van de siteverzameling of als lid van de groep eigenaren voor de site.</span><span class="sxs-lookup"><span data-stu-id="5c6bc-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="5c6bc-111">Zie voor meer informatie de [lijst toegang geweigerd tot aanvragen](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="5c6bc-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="5c6bc-112">Als een gebruiker het bericht ' toegang geweigerd ' heeft gekregen nadat deze uit Active Directory on-premises is verwijderd en daarna weer is toegevoegd, raadpleegt u [de toegang geweigerd wanneer een gebruikersaccount wordt gesynchroniseerd met Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="5c6bc-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

