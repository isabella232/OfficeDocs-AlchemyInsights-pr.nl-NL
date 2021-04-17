---
title: Automatische antwoorden instellen voor een postvak
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820929"
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
