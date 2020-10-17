---
title: 726 blokkeert het doorsturen van e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478339"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Doorsturen van e-mail blokkeren of de blokkering opheffen

Zie [doorsturen van E-mail configureren](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)om het doorsturen van e-mail voor een specifiek postvak in of uit te schakelen.

Op het tenantniveau wordt de besturing van extern doorsturen uitgevoerd met behulp van het uitgaande spam beleid. U kunt het uitgaande spamfilter beleid [hier](https://protection.office.com/antispam) of met de [opdracht Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)controleren.

Als u de volgende foutmelding ziet: **' 550 5.7.520 toegang geweigerd, uw organisatie mag niet extern doorsturen '**, Controleer of het beleid is geconfigureerd voor het inschakelen van extern automatisch doorsturen.

**Opmerking:** U wordt aangeraden de extern automatische doorstuur actie te behouden op het standaardbeleid voor het gebruik van uitgaande spamfilters en dit alleen in te schakelen voor de gebruikers die extern doorsturen willen maken door een aangepast beleid te maken voor deze gebruikers. Meer informatie vindt u in [externe e-mail forwarding configureren in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).