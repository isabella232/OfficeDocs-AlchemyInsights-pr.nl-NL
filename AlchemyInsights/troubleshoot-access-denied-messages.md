---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704889"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="fc771-102">Problemen met toegang geweigerde berichten oplossen</span><span class="sxs-lookup"><span data-stu-id="fc771-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="fc771-103">Als iemand het bericht 'Toegang geweigerd' heeft gekregen voor een gedeelde map in SharePoint, heeft de beheerder van de siteverzameling mogelijk vergrendelingsmodus voor gebruikersmachtigingen met beperkte toegang ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="fc771-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="fc771-104">Om dit uit te schakelen:</span><span class="sxs-lookup"><span data-stu-id="fc771-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="fc771-105">Blader naar de site, klik op het pictogram Instellingen en klik vervolgens op **Site-instellingen.**</span><span class="sxs-lookup"><span data-stu-id="fc771-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="fc771-106">Klik **onder Beheer van de siteverzameling** op Onderdelen van de **siteverzameling.**</span><span class="sxs-lookup"><span data-stu-id="fc771-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="fc771-107">Klik naast **de vergrendelingsmodus voor gebruikersmachtiging met** beperkte toegang op **Deactiveren.**</span><span class="sxs-lookup"><span data-stu-id="fc771-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="fc771-108">Het bericht Toegang geweigerd kan ook worden weergegeven voor gedeelde mappen als de site een publicerende site is.</span><span class="sxs-lookup"><span data-stu-id="fc771-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="fc771-109">Zie Toegang geweigerd bij [het openen van een gedeelde map voor meer informatie.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="fc771-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="fc771-110">Als iemand het bericht 'Toegang geweigerd' heeft gekregen bij het weergeven van toegangsaanvragen, moet de gebruiker worden toegevoegd als beheerder van een siteverzameling of als lid van de groep Eigenaren voor de site.</span><span class="sxs-lookup"><span data-stu-id="fc771-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="fc771-111">Zie de lijst Toegang tot [toegangsaanvragen geweigerd voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="fc771-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="fc771-112">Als een gebruiker het bericht 'Toegang geweigerd' heeft gekregen nadat deze on-premises uit Active Directory is verwijderd en vervolgens weer is toegevoegd, bekijkt u Toegang geweigerd wanneer een gebruikersaccount wordt gesynchroniseerd met [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="fc771-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

