---
title: Naamservers wijzigen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508083"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="9470b-102">De domeinnaamservers bijwerken zodat ze verwijzen naar Microsoft</span><span class="sxs-lookup"><span data-stu-id="9470b-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="9470b-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9470b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="9470b-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Microsoft 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="9470b-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="9470b-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="9470b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="9470b-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="9470b-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="9470b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9470b-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="9470b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9470b-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="9470b-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="9470b-110">Save changes.</span></span>

<span data-ttu-id="9470b-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen bij een domeinregistrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="9470b-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  