---
title: Problemen met geweigerde toegangs berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050700"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7ac9b-102">Problemen met geweigerde toegangs berichten oplossen</span><span class="sxs-lookup"><span data-stu-id="7ac9b-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7ac9b-103">Als iemand het bericht ' toegang geweigerd ' heeft gekregen voor een gedeelde map in SharePoint, heeft de beheerder van de siteverzameling mogelijk de vergrendelingsmodus voor beperkte toegang tot gebruikers machtiging ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7ac9b-104">Om dit uit te schakelen:</span><span class="sxs-lookup"><span data-stu-id="7ac9b-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7ac9b-105">Blader naar de site, klikt u op het pictogram instellingen en klik vervolgens op **site-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7ac9b-106">Klik onder **beheer van siteverzameling**op **site verzamelings functies**.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7ac9b-107">Klik naast **beperkte toegang tot de vergrendelingsmodus voor gebruikersmachtigingen**op **deactiveren**.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7ac9b-108">Een bericht toegang geweigerd kan ook optreden voor gedeelde mappen als de site een publicerende site is.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7ac9b-109">Zie [toegang geweigerd bij toegang tot een gedeelde map](https://go.microsoft.com/fwlink/?linkid=2004317)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="7ac9b-110">Als een persoon het bericht ' toegang geweigerd ' heeft gekregen bij het bekijken van toegangsverzoeken, moet de gebruiker worden toegevoegd als beheerder van een siteverzameling of als lid van de groep eigenaren voor de site.</span><span class="sxs-lookup"><span data-stu-id="7ac9b-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7ac9b-111">Zie voor meer informatie, [toegang geweigerd voor toegang tot Aanvragenlijst](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="7ac9b-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7ac9b-112">Als een gebruiker een bericht ' toegang geweigerd ' nadat ze zijn verwijderd uit Active Directory on-premises en vervolgens weer toegevoegd, Zie [toegang geweigerd wanneer een gebruikersaccount wordt gesynchroniseerd met Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="7ac9b-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

