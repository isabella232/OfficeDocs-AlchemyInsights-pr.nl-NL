---
title: Automatische antwoorden instellen voor een postvak
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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788877"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automatische antwoorden instellen voor het postvak van een gebruiker

**Methode 1**

1. Meld u aan bij de Microsoft 365-portal.

2. Ga naar **Gebruikers > Actieve gebruikers** (of **Groepen > Gedeelde postvakken** als u dit instelt voor een gedeeld postvak).

3. Selecteer een gebruiker met een Microsoft Exchange-postvak.

4. Ga in het flyoutmenu aan de rechterkant naar **E-mailinstellingen > Automatische antwoorden** (als het een gedeeld postvak is, klikt u gewoon op **Automatische antwoorden** in de flyout).

**Methode 2**

1. Meld u aan bij de Microsoft 365-beheerportal met uw beheerdersreferenties.

2. Vouw **Beheercentrums** uit en klik vervolgens op **Exchange**.

3. Klik in de rechterbovenhoek op de afbeelding, klik op **Andere gebruiker** en selecteer vervolgens het postvak van de gebruiker dat u wilt wijzigen.

4. Selecteer aan de linkerkant **Opties**, klik op **E-mail ordenen** en klik vervolgens op **Automatische antwoorden.**

**Methode 3**

Voer de volgende cmdlet uit in Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Zie [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) voor meer informatie over deze cmdlet.
