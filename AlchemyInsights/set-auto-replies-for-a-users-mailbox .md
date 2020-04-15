---
title: Automatische antwoorden instellen voor het postvak van een gebruiker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506455"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automatische antwoorden instellen voor het postvak van een gebruiker

**Methode 1**

1. Meld u aan bij de Office 365-portal.

2. Ga naar **Gebruikers > Actieve gebruikers** (of **Groepen > Gedeelde postvakken** als u dit instelt voor een gedeeld postvak).

3. Selecteer een gebruiker met een Microsoft Exchange-postvak.

4. Ga in het flyoutmenu aan de rechterkant naar **E-mailinstellingen > Automatische antwoorden** (als het een gedeeld postvak is, klikt u gewoon op **Automatische antwoorden** in de flyout).

**Methode 2**

1. Meld u aan bij de Office 365-beheerportal via beheerdersreferenties.

2. Vouw **Beheercentrums** uit en klik vervolgens op **Exchange**.

3. Klik in de rechterbovenhoek op de afbeelding, klik op **Andere gebruiker** en selecteer vervolgens het postvak van de gebruiker dat u wilt wijzigen.

4. Selecteer aan de linkerkant **Opties**, klik op **E-mail ordenen** en klik vervolgens op **Automatische antwoorden.**

**Methode 3**

Voer de volgende cmdlet uit in Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Zie [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) voor meer informatie over deze cmdlet.
