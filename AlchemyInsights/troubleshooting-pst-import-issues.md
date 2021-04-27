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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="9e498-102">Problemen oplossen bij het importeren van een PST-bestand</span><span class="sxs-lookup"><span data-stu-id="9e498-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="9e498-103">Zie Problemen met het importeren van een PST-bestand van Outlook oplossen als u importeert in de [Outlook-client zelf.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="9e498-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="9e498-104">Als u importservice gebruikt en deze vastzit, moet elk PST-bestand dat u uploadt naar de Azure Storage-locatie, niet groter zijn dan 20 GB.</span><span class="sxs-lookup"><span data-stu-id="9e498-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="9e498-105">PST-bestanden groter dan 20 GB kunnen van invloed zijn op de prestaties van het PST-importproces.</span><span class="sxs-lookup"><span data-stu-id="9e498-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="9e498-106">Zie Problemen die van invloed zijn op [pst-importtaken](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)voor meer informatie over het oplossen van problemen met vastgelopen taken.</span><span class="sxs-lookup"><span data-stu-id="9e498-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="9e498-107">Als u de status van een specifieke importklus wilt controleren, gebruikt [u Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)</span><span class="sxs-lookup"><span data-stu-id="9e498-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="9e498-108">Zie Overzicht van het importeren van pst-bestanden van uw organisatie voor meer informatie over de [importservice.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9e498-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
