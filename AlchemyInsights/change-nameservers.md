---
title: Naamservers wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818607"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="da2f2-102">De domeinnaamservers bijwerken zodat ze verwijzen naar Microsoft</span><span class="sxs-lookup"><span data-stu-id="da2f2-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="da2f2-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="da2f2-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="da2f2-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Microsoft 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="da2f2-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="da2f2-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="da2f2-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="da2f2-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="da2f2-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="da2f2-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="da2f2-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="da2f2-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="da2f2-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="da2f2-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="da2f2-110">Save changes.</span></span>

<span data-ttu-id="da2f2-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen bij een domeinregistrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="da2f2-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  