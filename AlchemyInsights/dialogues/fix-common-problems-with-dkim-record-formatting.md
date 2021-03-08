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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523747"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Veelvoorkomende problemen met DKIM-recordopmaak oplossen

De meeste DKIM-instellingen hebben betrekking op onjuiste DNS-records.

U lost de problemen met de DKIM-set-up op door te controleren of de DKIM CNAME-record **(geen** TXT-record) juist is opgemaakt. Zie Wat u moet doen om DKIM handmatig in te stellen [in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)voor meer informatie.

Zie DNS-records maken bij een [DNS-hostingprovider voor Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)als u in het algemeen hulp nodig hebt met DNS-records.

> [!NOTE]
> Nadat u uw DKIM DNS-records bij de DNS-hostingservice voor uw domein hebt gemaakt of bijgewerkt, moet u wachten totdat de DNS-records zijn doorgegeven.
