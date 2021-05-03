---
title: Problemen met de importservice-taak blijven hangen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124918"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="005e0-102">Problemen met de importservice-taak blijven hangen</span><span class="sxs-lookup"><span data-stu-id="005e0-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="005e0-103">Als u problemen ondervindt met Het importeren van servicetaken blijft hangen of mislukt, bekijkt u het volgende en probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="005e0-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="005e0-104">Controleer de grootte van het PST-bestand.</span><span class="sxs-lookup"><span data-stu-id="005e0-104">Review the size of of the PST file.</span></span> <span data-ttu-id="005e0-105">De maximale aanbevolen grootte van een PST-bestand voor importeren is 20 GB.</span><span class="sxs-lookup"><span data-stu-id="005e0-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="005e0-106">Als u vermoedt dat items zijn overgeslagen vanwege beschadiging, kunt u Scanpst.exe om fouten in PST-bestanden te diagnosticeren en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="005e0-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="005e0-107">Als u tijdens het importeren een foutmelding 'MapiExceptionShutoffQuotaExceeded' ziet, moet u ervoor zorgen dat het doelpostvak voldoende capaciteit heeft om de gewenste PST-bestanden te importeren.</span><span class="sxs-lookup"><span data-stu-id="005e0-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="005e0-108">Zie Problemen met pst-importtaken oplossen voor meer informatie over het oplossen van problemen met [pst-importtaken.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="005e0-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="005e0-109">Zie Problemen met het importeren van een PST-bestand [(Outlook .pst-bestand (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)oplossen voor informatie over het oplossen van problemen bij het importeren van PST's in Outlook.</span><span class="sxs-lookup"><span data-stu-id="005e0-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>