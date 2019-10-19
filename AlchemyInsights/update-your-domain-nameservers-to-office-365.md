---
title: De domeinnaamservers voor Office 365 bijwerken
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742170"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="dfcb4-102">De domeinnaamservers voor Office 365 bijwerken</span><span class="sxs-lookup"><span data-stu-id="dfcb4-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="dfcb4-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="dfcb4-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="dfcb4-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Office 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="dfcb4-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="dfcb4-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="dfcb4-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="dfcb4-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="dfcb4-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="dfcb4-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="dfcb4-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="dfcb4-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="dfcb4-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="dfcb4-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="dfcb4-110">Save changes.</span></span>

<span data-ttu-id="dfcb4-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen voor het instellen van Office 365 bij een domeinregistrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="dfcb4-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  