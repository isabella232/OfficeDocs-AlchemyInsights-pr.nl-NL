---
title: De domeinnaamservers bijwerken zodat ze verwijzen naar Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734906"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="af27e-102">De domeinnaamservers bijwerken zodat ze verwijzen naar Microsoft</span><span class="sxs-lookup"><span data-stu-id="af27e-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="af27e-103">Opmerking: het kan soms 48 uur duren voordat wijzigingen in naamservers zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="af27e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="af27e-104">Voor het instellen van uw domein met Microsoft moet de naamservers voor uw registratieservice worden bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="af27e-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="af27e-105">Maak uw naamserverrecords bij uw domeinregistrar of bewerk ze.</span><span class="sxs-lookup"><span data-stu-id="af27e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="af27e-106">Ga naar de website van uw domeinregistrar en zoek het gedeelte waar u de naamservers kunt bewerken.</span><span class="sxs-lookup"><span data-stu-id="af27e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="af27e-107">Maak twee naamserverrecords of werk ze bij zodat ze overeenkomen met de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="af27e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="af27e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af27e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="af27e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af27e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="af27e-110">Sla de wijzigingen op.</span><span class="sxs-lookup"><span data-stu-id="af27e-110">Save changes.</span></span>

<span data-ttu-id="af27e-111">U kunt ook gedetailleerde instructies vinden in dit artikel: [Naamservers wijzigen voor het instellen van Microsoft 365 met een domeinregistratie](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="af27e-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  