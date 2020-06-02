---
title: Map 1336 RecoverableItems is vol
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510747"
---
# <a name="the-recoverable-items-folder-is-full"></a>De map Herstelbare items is vol

Voor Exchange Online-postvakken is de standaardopslaglimiet voor de map Herstelbare items 30 GB. De opslaglimiet voor de map Herstelbare items wordt automatisch verhoogd tot 100 GB als het postvak wordt geplaatst in Litigation Hold, eDiscovery hold of is toegewezen aan een bewaarbeleid.

Wanneer de map Herstelbare items de opslaglimiet bereikt, wordt de functionaliteit van het postvak op de volgende manieren beïnvloed:

- De gebruiker kan geen items uit het postvak verwijderen.

- De assistent voor beheerde mappen kan items niet verwijderen op basis van bewaartag of instellingen voor beheerde mappen.

- Voor postvakken waarvoor single itemherstel is ingeschakeld of in de wacht wordt gezet, kan het proces voor kopieerpaginabeveiliging geen versies van door de gebruiker bewerkte items onderhouden.

- Voor postvakken waarvoor postvakcontroleregistratie is ingeschakeld, kunnen geen logboekgegevens van postvakken worden opgeslagen in de submap Audits in de map Herstelbare items.

Voor postvakken die niet in de wacht staan, kunnen beheerders de opdracht in Exchange Online PowerShell gebruiken `Search-Mailbox -SearchDumpsterOnly -DeleteContent` om items in de map Herstelbare items te verwijderen. Lees de volgende onderwerpen voor meer informatie:

- [Berichten zoeken en verwijderen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Zoekpostvak](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Voor postvakken die in de wacht staan, moeten beheerders de wachtruimte verwijderen voordat ze items uit de map Herstelbare items kunnen verwijderen. Zie [Items verwijderen in de map Herstelbare items van postvakken in de cloud in de wachtstand](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)voor meer informatie.

Om te voorkomen dat de map Herstelbare items vol raakt, kunnen beheerders de opslaglimiet van de map Herstelbare items voor postvakken in de wacht verhogen en een beleid voor het bewaren van postvakken instellen dat items verplaatst vanuit de map Herstelbare items naar het archiefpostvak van de gebruiker. Zie [Het quotum herstelbare items voor postvakken in de wacht vergroten](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
