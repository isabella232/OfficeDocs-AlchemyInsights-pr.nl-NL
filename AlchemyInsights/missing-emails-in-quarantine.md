---
title: Ontbrekende e-mailberichten in quarantaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539819"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mailberichten in quarantaine"

Beheerders kunnen [deze berichten bekijken,](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files) vrijgeven of verwijderen.

Als u het beveiligingscentrum & compliancecentrum wilt openen, gaat u naar [https://protection.office.com](https://protection.office.com/) . Als u de pagina Quarantaine rechtstreeks wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

U kunt zoeken op een van de volgende waarden:  

- **Bericht-ID**: de wereldwijd unieke identificatie van het bericht. Als u een bericht in de lijst selecteert, wordt de waarde  **Bericht-id**  weergegeven in het flyoutvenster  **Details**  dat wordt weergegeven. Beheerders kunnen [berichttracering](/microsoft-365/security/office-365-security/message-trace-scc) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.
- **E-mailadres afzender**: een enkel e-mailadres van een afzender.
- **E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.
- **Onderwerp**: gebruik het volledige onderwerp van het bericht. De zoekopdracht is niet hoofdlettergevoelig.

Nadat u de zoekcriteria hebt opgegeven, klikt u op de ![Knop vernieuwen](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Vernieuwen** om de resultaten te filteren.

De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine zijn:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Deze cmdlet is alleen voor berichten, niet voor malwarebestanden van Microsoft Defender voor Office 365 voor SharePoint Online, OneDrive voor Bedrijven of Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)