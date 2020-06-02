---
title: Foutcode 550 5.7.501 Toegang geweigerd, spammisbruik ontdekt
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 9fd4f14798f27e7bf93daceb3620aff9b7f9e8ed
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506805"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Toegang geweigerd, spammisbruik ontdekt

Dit bericht treedt meestal op wanneer gebruikers e-mailberichten verzenden vanaf IP-adressen met behulp van het oorspronkelijke *.onmicrosoft.com-domein* dat is toegewezen aan nieuwe tenants in Microsoft 365. De eenvoudigste manier om dit probleem op te lossen is:

1. [Een domein toevoegen aan uw tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Wijzig het primaire e-mailadres](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) van uw gebruikers in het nieuwe aangepaste domein dat u zojuist hebt toegevoegd.
