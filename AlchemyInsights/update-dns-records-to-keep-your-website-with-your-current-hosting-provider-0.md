---
title: DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353172"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="1ef07-102">DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden</span><span class="sxs-lookup"><span data-stu-id="1ef07-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="1ef07-103">Op de pagina [Domeinen](https://portal.office.com/adminportal/home#/Domains) selecteert u in de lijst met domeinen het domein dat u voor uw website gebruikt en selecteert u vervolgens **DNS-instellingen** in het deelvenster Beheren.</span><span class="sxs-lookup"><span data-stu-id="1ef07-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="1ef07-104">Selecteer **+ Nieuwe aangepaste record** en typ het volgende:</span><span class="sxs-lookup"><span data-stu-id="1ef07-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1ef07-105">Voor **DNS-type** voert u in: **A (adres)**</span><span class="sxs-lookup"><span data-stu-id="1ef07-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="1ef07-106">Typ het volgende voor **Hostnaam of alias**: **@**</span><span class="sxs-lookup"><span data-stu-id="1ef07-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="1ef07-107">Voor **IP-adres** typt u het statische IP-adres van uw website waar deze momenteel wordt gehost (bijvoorbeeld: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="1ef07-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="1ef07-p101">Dit moet een  *statisch*  IP-adres van de website zijn, geen  *dynamisch*  IP-adres. Kijk op de site waar uw website wordt gehost om er zeker van te zijn dat u een statisch IP-adres kunt krijgen voor uw openbare website.</span><span class="sxs-lookup"><span data-stu-id="1ef07-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="1ef07-110">Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="1ef07-110">Select **Save**.</span></span>

<span data-ttu-id="1ef07-111">U kunt eveneens een CNAME-record maken om klanten te helpen bij het zoeken van uw website.</span><span class="sxs-lookup"><span data-stu-id="1ef07-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="1ef07-112">Selecteer **+ Nieuwe aangepaste record** en typ het volgende:</span><span class="sxs-lookup"><span data-stu-id="1ef07-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1ef07-113">Voor **DNS-type** voert u in: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="1ef07-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="1ef07-114">Voor **Hostnaam of alias** typt u: **www**</span><span class="sxs-lookup"><span data-stu-id="1ef07-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="1ef07-115">Voor **Adres waarnaar wordt verwezen** typt u de FQDN (Fully Qualified Domain Name) voor uw website (bijvoorbeeld contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1ef07-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="1ef07-116">Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="1ef07-116">Select **Save**.</span></span>
