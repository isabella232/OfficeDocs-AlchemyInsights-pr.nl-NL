---
title: Ontbrekende e-mails in quarantaine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569047"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mails in quarantaine"

Beheerders kunnen [deze berichten bekijken, vrijgeven of verwijderen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

& Ga naar [https://protection.office.com](https://protection.office.com/) . Als u de quarantainepagina rechtstreeks wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

U kunt zoeken op een van de volgende waarden:  

- **Bericht-ID**: de wereldwijd unieke identificatie van het bericht. Als u een bericht in de lijst selecteert, wordt de waarde **bericht-id** weergegeven in het flyoutvenster **Details** dat wordt weergegeven. Beheerders kunnen [berichttracering](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.
- **E-mailadres afzender**: een enkel e-mailadres van een afzender.
- **E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.
- **Onderwerp**: gebruik het volledige onderwerp van het bericht. De zoekopdracht is niet hoofdlettergevoelig.

Nadat u de zoekcriteria hebt ingevoerd, klikt u op ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Vernieuwen** om de resultaten te filteren.  

De cmdlets die u gebruikt om berichten en bestanden in quarantaine te bekijken en te beheren zijn:
- [Bericht in quarantaine verwijderen](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [In quarantaine exporterenMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [In quarantaine plaatsenMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Houd er rekening mee dat deze cmdlet alleen is voor berichten, niet voor malwarebestanden van ATP voor SharePoint Online, OneDrive voor Bedrijven of Teams.
- [Release-quarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)