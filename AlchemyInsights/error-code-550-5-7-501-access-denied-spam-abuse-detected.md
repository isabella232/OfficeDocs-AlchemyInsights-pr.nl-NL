---
title: Foutcode 550 5.7.501 Toegang geweigerd, spammisbruik gedetecteerd
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044263"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Toegang geweigerd, spammisbruik gedetecteerd

Dit bericht treedt meestal op wanneer gebruikers e-mailberichten verzenden van IP-adressen met het eerste *.onmicrosoft.com-domein* dat is toegewezen aan nieuwe tenants in Microsoft 365. De eenvoudigste manier om dit probleem op te lossen is door:

1. [Voeg een domein toe aan uw tenant.](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)

2. [Wijzig het primaire e-mailadres van uw gebruikers](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) in het nieuwe aangepaste domein dat u zojuist hebt toegevoegd.
