---
title: Problemen oplossen bij het importeren van een PST-bestand
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
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059810"
---
# <a name="troubleshooting-pst-import-issues"></a>Problemen oplossen bij het importeren van een PST-bestand

- Zie Problemen met het importeren van een PST-bestand van Outlook oplossen als u importeert in de [Outlook-client zelf.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Als u importservice gebruikt en deze vastzit, moet elk PST-bestand dat u uploadt naar de Azure Storage-locatie, niet groter zijn dan 20 GB. PST-bestanden groter dan 20 GB kunnen van invloed zijn op de prestaties van het PST-importproces. Zie Problemen die van invloed zijn op [pst-importtaken](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)voor meer informatie over het oplossen van problemen met vastgelopen taken.

- Als u de status van een specifieke importklus wilt controleren, gebruikt [u Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Zie Overzicht van het importeren van pst-bestanden van uw organisatie voor meer informatie over de [importservice.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
