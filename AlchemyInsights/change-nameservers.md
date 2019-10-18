---
title: Naamservers wijzigen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736644"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="91f85-102">De domeinnaamservers voor Office 365 bijwerken</span><span class="sxs-lookup"><span data-stu-id="91f85-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="91f85-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="91f85-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="91f85-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Office 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="91f85-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="91f85-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="91f85-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="91f85-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="91f85-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="91f85-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91f85-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="91f85-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91f85-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="91f85-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="91f85-110">Save changes.</span></span>

<span data-ttu-id="91f85-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen voor het instellen van Office 365 bij een domeinregistrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="91f85-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  