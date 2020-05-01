---
title: Problemen oplossen bij het importeren van een PST-bestand
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991154"
---
# <a name="troubleshooting-pst-import-issues"></a>Problemen oplossen bij het importeren van een PST-bestand

- Als u in de Outlook-client zelf importeert, raadpleegt u [Problemen oplossen bij het importeren van een .pst-bestand van Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Als u de importservice gebruikt en de service is vastgelopen, moet u er rekening mee houden dat elk .pst-bestand dat u uploadt naar de Azure Storage-locatie, niet groter mag zijn dan 20 GB. PST-bestanden die groter zijn dan 20 GB, beïnvloeden mogelijk de prestaties van het PST-importproces.

- Als u de status van een bepaalde importtaak wilt controleren, kunt u [Get-MailboxImportRequest -batchnaam](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) gebruiken.

- Zie [Overzicht van het importeren van de PST-bestanden van uw organisatie](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide) voor de volledige informatie over de importservice.
