---
title: de map 1336 RecoverableItems is vol
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741262"
---
# <a name="the-recoverable-items-folder-is-full"></a>De map herstelbare items is vol

Voor postvakken van Exchange Online is de standaardopslagruimte voor de map herstelbare items 30 GB. De opslaglimiet voor de map herstelbare items wordt automatisch verhoogd naar 100 GB als het postvak wordt geplaatst op een gerechtelijke, eDiscovery-bewaring of aan een bewaarbeleid.

Wanneer de map herstelbare items de opslaglimiet bereikt, heeft dit gevolgen voor de functionaliteit van het postvak op de volgende manieren:

- De gebruiker kan items uit het postvak niet verwijderen.

- De Instellingsassistent voor beheerde mappen kan geen items verwijderen op basis van het Bewaar label of de instellingen van de beheerde map.

- Voor postvakken waarop eenmalige items hersteld zijn of die in de wachtstand staan, kunnen de versies van door de gebruiker bewerkte pagina's niet worden bijgehouden.

- Voor postvakken met een auditlogboek voor Postvak in, kunnen auditlogboek vermeldingen van het postvak niet worden opgeslagen in de submap audits in de map herstelbare items.

Voor postvakken die niet in bewaring zijn, kunnen beheerders de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` opdracht in PowerShell van Exchange Online gebruiken om items in de map herstelbare items te verwijderen. Zie de volgende onderwerpen voor meer informatie:

- [Berichten zoeken en verwijderen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Zoeken-Postvak](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Voor postvakken die in de wacht staan, moeten beheerders de bewaring verwijderen voordat ze items kunnen verwijderen uit de map herstelbare items. Zie voor meer informatie [items verwijderen in de map herstelbare items van de Cloud postvakken in bewaring](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Om te voorkomen dat de map herstelbare items volledig wordt, kan het zijn dat beheerders de opslaglimiet van de map herstelbare items voor postvakken in de wacht zetten en het bewaarbeleid voor Postvak in instellen voor het opslaan van items in de map herstelbare items in het archief postvak van de gebruiker. Zie [het quotum voor herstelbare items voor postvakken in de wacht zetten](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
