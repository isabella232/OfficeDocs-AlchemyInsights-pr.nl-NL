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
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706750"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="68a86-102">De domeinnaamservers bijwerken zodat ze verwijzen naar Microsoft</span><span class="sxs-lookup"><span data-stu-id="68a86-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="68a86-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="68a86-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="68a86-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Microsoft 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="68a86-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="68a86-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="68a86-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="68a86-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="68a86-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="68a86-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="68a86-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="68a86-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="68a86-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="68a86-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="68a86-110">Save changes.</span></span>

<span data-ttu-id="68a86-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen bij een domeinregistrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="68a86-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  