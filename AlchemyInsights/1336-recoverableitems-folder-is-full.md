---
title: 1336 RecoverableItems map is vol
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284064"
---
# <a name="the-recoverable-items-folder-is-full"></a>De herstelbare Items map is vol

Voor de Exchange Online-postvakken in Office 365 is de standaard opslaglimiet voor de map herstelbare Items 30 GB. De opslaglimiet voor de map herstelbare Items automatisch verhoogd naar 100 GB als het postvak op de rechtszaak houdt, eDiscovery-wacht wordt geplaatst of is toegewezen aan een bewaarbeleid Office 365.
  
Als de map herstelbare Items de opslaglimiet bereikt, postbus functionaliteit is waarin dit probleem optreedt op de volgende manieren:
  
- De gebruiker kan items uit het postvak verwijderen.
    
- De beheerde Mapassistent verwijderen artikelen op basis van inhoudingen tag of instellingen van beheerde mappen niet.
    
- Voor postvakken die één Item herstellen ingeschakeld of in de wachtstand worden geplaatst, kan niet de bescherming pagina kopiëren tijdens het schrijven proces versies van items bewerkt door de gebruiker onderhouden.
    
- Voor postvakken die postbus controlegebeurtenissen vastleggen is ingeschakeld, kunnen geen logboekvermeldingen postbus controle worden opgeslagen in de submap kunnen worden opgeslagen in de map Items terug te vorderen.
    
Postvakken die niet in de wachtstand, beheerders kunt gebruiken de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` opdracht in Exchange Online PowerShell verwijderen van items in de map Items terug te vorderen. Zie de volgende onderwerpen voor meer informatie: 
  
- [Zoek en verwijder berichten](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Zoeken-postbus](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Voor postbussen die geblokkeerd zijn, moeten beheerders de blokkering verwijderen voordat ze verwijderde items uit de map Items terug te vorderen kunnen. Zie de [items in de map van de postvakken op cloud-gebaseerde houdt herstelbare Items verwijderen](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)voor meer informatie.
  
Om te voorkomen dat de herstelbare Items map vol raken, kan beheerders de opslaglimiet van de herstelbare Items, map voor postvakken op houdt en instellen van een postbus bewaarbeleid die items uit de map herstelbare Items naar het archief van de gebruiker verplaatst toenemen postbus. Zie het [verhogen van de herstelbare Items voor postvakken op houdt](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

