---
title: Externe automatische e-mail doorsturen blokkeren of deblokkeren
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315869"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Eeuwig automatisch doorsturen van e-mail blokkeren of deblokkeren

Zie E-mail doorsturen configureren als u het doorsturen van e-mail voor een specifiek postvak wilt in- [of uitschakelen.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Beheerders kunnen externe doorsturen voor de organisatie beheren met behulp van [uitgaand spambeleid.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) U beheert uitgaand spambeleid in de Microsoft 365 Defender portal op of met de <https://security.microsoft.com/antispam> [cmdlet Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) in Exchange Online PowerShell.

Als u de volgende foutmelding ontvangt: **'550 5.7.520 Access geweigerd,** Uw organisatie staat extern doorsturen niet toe', zorg er dan voor dat het beleid is geconfigureerd voor het inschakelen van externe, automatisch doorgestuurde berichten.

**Opmerking:** We hebben de standaardwaarde Automatisch  **aanbevolen:** systeem dat is ingesteld voor de instelling Voor automatisch doorsturen van regels in uw standaardbeleid voor uitgaande spamfilters (automatisch extern doorsturen is geblokkeerd; interne automatische doorsturen werkt nog steeds). U moet aangepaste beleidsregels voor uitgaand spamfilter maken en de waarde **Aan - Doorsturen alleen** gebruiken voor gebruikers die externe automatische e-mail doorsturen nodig hebben. Zie Externe e-mail doorsturen [configureren in](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)Office 365.
