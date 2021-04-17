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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden

1. Ga in het Microsoft 365-beheercentrum naar de pagina **Domeinen** instellen en selecteer in de lijst met domeinen het domein dat u voor uw  >  [](https://admin.microsoft.com/Adminportal#/Domains) website gebruikt.

2. Selecteer **+ Nieuwe aangepaste record** en typ het volgende:

  - Voor **DNS-type** voert u in: **A (adres)**

  - Typ het volgende voor **Hostnaam of alias**: **@**

  - Voor **IP-adres** typt u het statische IP-adres van uw website waar deze momenteel wordt gehost (bijvoorbeeld: 172.16.140.1).

    Dit moet een  *statisch*  IP-adres van de website zijn, geen  *dynamisch*  IP-adres. Kijk op de site waar uw website wordt gehost om er zeker van te zijn dat u een statisch IP-adres kunt krijgen voor uw openbare website.

3. Selecteer **Opslaan**.

U kunt eveneens een CNAME-record maken om klanten te helpen bij het zoeken van uw website.
  
1. Selecteer **+ Nieuwe aangepaste record** en typ het volgende:

  - Voor **DNS-type** voert u in: **CNAME (alias)**

  - Voor **Hostnaam of alias** typt u: **www**

  - Voor **Adres waarnaar wordt verwezen** typt u de FQDN (Fully Qualified Domain Name) voor uw website (bijvoorbeeld contoso.com).

2. Selecteer **Opslaan**.
