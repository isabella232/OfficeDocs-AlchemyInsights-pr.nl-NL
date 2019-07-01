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
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363072"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="fc3c6-102">De domeinnaamservers voor Office 365 bijwerken</span><span class="sxs-lookup"><span data-stu-id="fc3c6-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="fc3c6-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="fc3c6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="fc3c6-p101">De naamservers bij uw registrar moeten worden bijgewerkt als u uw domein in Office 365 wilt instellen. Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="fc3c6-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="fc3c6-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="fc3c6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="fc3c6-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="fc3c6-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="fc3c6-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fc3c6-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="fc3c6-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fc3c6-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="fc3c6-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="fc3c6-110">Save changes.</span></span>

<span data-ttu-id="fc3c6-111">Gedetailleerde instructies kunt u ook in het volgende artikel vinden: [Naamservers wijzigen voor het instellen van Office 365 bij een domeinregistrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="fc3c6-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  