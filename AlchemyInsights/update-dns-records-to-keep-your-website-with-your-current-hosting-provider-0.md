---
title: DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827508"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="9bfb7-102">DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden</span><span class="sxs-lookup"><span data-stu-id="9bfb7-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="9bfb7-103">Ga in het Microsoft 365-beheercentrum naar de pagina **Domeinen** instellen en selecteer in de lijst met domeinen het domein dat u voor uw  >  [](https://admin.microsoft.com/Adminportal#/Domains) website gebruikt.</span><span class="sxs-lookup"><span data-stu-id="9bfb7-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="9bfb7-104">Selecteer **+ Nieuwe aangepaste record** en typ het volgende:</span><span class="sxs-lookup"><span data-stu-id="9bfb7-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9bfb7-105">Voor **DNS-type** voert u in: **A (adres)**</span><span class="sxs-lookup"><span data-stu-id="9bfb7-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="9bfb7-106">Typ het volgende voor **Hostnaam of alias**: **@**</span><span class="sxs-lookup"><span data-stu-id="9bfb7-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="9bfb7-107">Voor **IP-adres** typt u het statische IP-adres van uw website waar deze momenteel wordt gehost (bijvoorbeeld: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="9bfb7-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="9bfb7-p101">Dit moet een  *statisch*  IP-adres van de website zijn, geen  *dynamisch*  IP-adres. Kijk op de site waar uw website wordt gehost om er zeker van te zijn dat u een statisch IP-adres kunt krijgen voor uw openbare website.</span><span class="sxs-lookup"><span data-stu-id="9bfb7-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="9bfb7-110">Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="9bfb7-110">Select **Save**.</span></span>

<span data-ttu-id="9bfb7-111">U kunt eveneens een CNAME-record maken om klanten te helpen bij het zoeken van uw website.</span><span class="sxs-lookup"><span data-stu-id="9bfb7-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="9bfb7-112">Selecteer **+ Nieuwe aangepaste record** en typ het volgende:</span><span class="sxs-lookup"><span data-stu-id="9bfb7-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9bfb7-113">Voor **DNS-type** voert u in: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="9bfb7-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="9bfb7-114">Voor **Hostnaam of alias** typt u: **www**</span><span class="sxs-lookup"><span data-stu-id="9bfb7-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="9bfb7-115">Voor **Adres waarnaar wordt verwezen** typt u de FQDN (Fully Qualified Domain Name) voor uw website (bijvoorbeeld contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9bfb7-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="9bfb7-116">Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="9bfb7-116">Select **Save**.</span></span>
