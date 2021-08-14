---
title: Veelvoorkomende problemen met DKIM-recordopmaak oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930056"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Veelvoorkomende problemen met DKIM-recordopmaak oplossen

De meeste DKIM-instellingen zijn gerelateerd aan onjuiste DNS-records.

Als u de DKIM-set-upproblemen wilt oplossen, controleert u of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt. Zie Wat u moet doen [om DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)handmatig in te stellen in Office 365.

Als u hulp nodig hebt bij DNS-records in het algemeen, zie [DNS-records maken bij een DNS-hostingprovider voor Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Nadat u uw DKIM DNS-records bij de DNS-hostingservice voor uw domein hebt gemaakt of bijgewerkt, moet u wachten totdat de DNS-records worden doorgegeven.
