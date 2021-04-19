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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826158"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="66dee-102">Problemen oplossen bij het importeren van een PST-bestand</span><span class="sxs-lookup"><span data-stu-id="66dee-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="66dee-103">Als u in de Outlook-client zelf importeert, raadpleegt u [Problemen oplossen bij het importeren van een .pst-bestand van Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="66dee-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="66dee-104">Als u de importservice gebruikt en de service is vastgelopen, moet u er rekening mee houden dat elk .pst-bestand dat u uploadt naar de Azure Storage-locatie, niet groter mag zijn dan 20 GB.</span><span class="sxs-lookup"><span data-stu-id="66dee-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="66dee-105">PST-bestanden die groter zijn dan 20 GB, beïnvloeden mogelijk de prestaties van het PST-importproces.</span><span class="sxs-lookup"><span data-stu-id="66dee-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="66dee-106">Als u de status van een bepaalde importtaak wilt controleren, kunt u [Get-MailboxImportRequest -batchnaam](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) gebruiken.</span><span class="sxs-lookup"><span data-stu-id="66dee-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="66dee-107">Zie [Overzicht van het importeren van de PST-bestanden van uw organisatie](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide) voor de volledige informatie over de importservice.</span><span class="sxs-lookup"><span data-stu-id="66dee-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
