---
title: DKIM instellen met aangepaste domeinen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744090"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM instellen met aangepaste domeinen

U moet twee CNAME-records publiceren voor elk aangepast domein in DNS. Gebruik hiervoor de volgende indeling:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** is de tekst links van **.mail.protection.outlook.com** in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld contoso-com voor het **domein contoso.com).** **InitialDomain** is het domein dat u hebt gebruikt toen u zich hebt aangemeld voor Office 365 **(bijvoorbeeld contoso.onmicrosoft.com).**

Zie DNS-records maken bij een [DNS-hostingprovider voor Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)voor meer informatie over DNS-records.