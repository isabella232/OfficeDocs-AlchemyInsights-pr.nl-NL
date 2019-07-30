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
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925280"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden

1. Selecteer op de pagina [domeinen](https://portal.office.com/adminportal/home#/Domains) in de lijst met domeinen het domein dat u voor uw website gebruikt.

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
