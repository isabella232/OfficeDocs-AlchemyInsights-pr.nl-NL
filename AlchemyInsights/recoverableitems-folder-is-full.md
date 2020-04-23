---
title: 1336 Map RecoverableItems is vol
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
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720247"
---
# <a name="the-recoverable-items-folder-is-full"></a>De map Herstelbare items is vol

Voor Exchange Online-postvakken is de standaardopslaglimiet voor de map Herstelbare items 30 GB. De opslaglimiet voor de map Herstelbare items wordt automatisch verhoogd tot 100 GB als het postvak wordt geplaatst in De wachtruimte voor geschillen, eDiscovery-blokkering of is toegewezen aan een bewaarbeleid.

Wanneer de map Herstelbare items de opslaglimiet bereikt, wordt de postvakfunctionaliteit op de volgende manieren beïnvloed:

- De gebruiker kan items niet uit het postvak verwijderen.

- De beheerde mapassistent kan items niet verwijderen op basis van bewaartag of beheerde mapinstellingen.

- Voor postvakken waarvoor herstel met één item is ingeschakeld of in de wachtstand is geplaatst, kan het kopieer-on-write-paginabeveiligingsproces geen versies van items onderhouden die door de gebruiker zijn bewerkt.

- Voor postvakken waarvoor logboekregistratie voor postvakcontrole is ingeschakeld, kunnen geen postvakcontrolelogboekvermeldingen worden opgeslagen in de submap Audits in de map Herstelbare items.

Voor postvakken die niet in de wacht `Search-Mailbox -SearchDumpsterOnly -DeleteContent` staan, kunnen beheerders de opdracht in Exchange Online PowerShell gebruiken om items in de map Herstelbare items te verwijderen. Lees de volgende onderwerpen voor meer informatie:

- [Berichten zoeken en verwijderen](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Zoekpostvak](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Voor postvakken die in de wachtstaan, moeten beheerders de blokkering verwijderen voordat ze items uit de map Herstelbare items kunnen verwijderen. Zie [Items verwijderen in de map Items met herstelbare items in de wachtstand](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)in de cloud voor meer informatie.

Om te voorkomen dat de map Herstelbare items vol raakt, kunnen beheerders de opslaglimiet van de map Herstelbare items voor postvakine in de wacht zetten en een postvakbehoudbeleid instellen dat items van de map Herstelbare items naar het archiefpostvak van de gebruiker verplaatst. Zie [Het quotum voor herstelbare items voor postvak in de wacht verhogen](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
