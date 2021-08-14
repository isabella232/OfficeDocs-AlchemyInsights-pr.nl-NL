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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972414"
---
# <a name="troubleshooting-pst-import-issues"></a>Problemen oplossen bij het importeren van een PST-bestand

- Als u importeert in de Outlook client zelf, zie Problemen met het importeren van een [PST-bestand](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)Outlook oplossen.

- Als u importservice gebruikt en deze vastzit, moet elk PST-bestand dat u uploadt naar de Azure Storage niet groter zijn dan 20 GB. PST-bestanden groter dan 20 GB kunnen van invloed zijn op de prestaties van het PST-importproces. Zie Problemen die van invloed zijn op [pst-importtaken](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)voor meer informatie over het oplossen van problemen met vastgelopen taken.

- Als u de status van een specifieke importklus wilt controleren, gebruikt [u Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Zie Overzicht van het importeren van pst-bestanden van uw organisatie voor meer informatie over de [importservice.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
