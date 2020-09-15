---
title: Ontbrekende e-mailberichten in quarantaine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673709"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mailberichten in quarantaine

Beheerders kunnen [deze berichten weergeven, vrijgeven of verwijderen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Als u het beveiligings & nalevings centrum wilt openen, gaat u naar [https://protection.office.com](https://protection.office.com/) . Als u de quarantaine pagina direct wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

U kunt zoeken op een van de volgende waarden:  

- **Bericht-ID**: de wereldwijd unieke identificatie van het bericht. Als u een bericht in de lijst selecteert, wordt de waarde van de  **bericht-id**  weergegeven in het deelvenster  **Details**  van het bericht dat wordt weergegeven. Beheerders kunnen [berichttracering](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.
- **E-mailadres afzender**: een enkel e-mailadres van een afzender.
- **E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.
- **Onderwerp**: gebruik het volledige onderwerp van het bericht. De zoekopdracht is niet hoofdlettergevoelig.

Nadat u de zoekcriteria hebt ingevoerd, klikt u op ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **vernieuwen** om de resultaten te filteren.  

De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine, zijn:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Voorbeeld: QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): deze cmdlet is alleen voor berichten, geen malware-bestanden uit de ATP voor SharePoint Online, OneDrive voor bedrijven of teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)