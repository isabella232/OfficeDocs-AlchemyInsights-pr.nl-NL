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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831729"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mailberichten in quarantaine"

Beheerders kunnen [deze berichten bekijken,](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide) vrijgeven of verwijderen.

Als u het beveiligingscentrum & compliancecentrum wilt openen, gaat u naar [https://protection.office.com](https://protection.office.com/) . Als u de pagina Quarantaine rechtstreeks wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

U kunt zoeken op een van de volgende waarden:  

- **Bericht-ID**: de wereldwijd unieke identificatie van het bericht. Als u een bericht in de lijst selecteert, wordt de waarde  **Bericht-id**  weergegeven in het flyoutvenster  **Details**  dat wordt weergegeven. Beheerders kunnen [berichttracering](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.
- **E-mailadres afzender**: een enkel e-mailadres van een afzender.
- **E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.
- **Onderwerp**: gebruik het volledige onderwerp van het bericht. De zoekopdracht is niet hoofdlettergevoelig.

Nadat u de zoekcriteria hebt ingevoerd, klikt u op ![ Knop Vernieuwen vernieuwen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **om** de resultaten te filteren.  

De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine zijn:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Deze cmdlet is alleen voor berichten, niet voor malwarebestanden van ATP voor SharePoint Online, OneDrive voor Bedrijven of Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)