---
title: Voor de migratiebatch Openbare map met de status Voltooid met fouten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158597"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="2b987-102">Voor de migratiebatch Openbare map met de status Voltooid met fouten</span><span class="sxs-lookup"><span data-stu-id="2b987-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="2b987-103">Gebruik de volgende stappen om de batch te voltooien en sla de grote/slechte items over:</span><span class="sxs-lookup"><span data-stu-id="2b987-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="2b987-104">De overgeslagen items op de migratiebatch goedkeuren:</span><span class="sxs-lookup"><span data-stu-id="2b987-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="2b987-105">Gebruik de volgende opdracht om de overgeslagen items op migratieverzoeken goed te keuren die zijn 'Gesynchroniseerd' maar niet zijn voltooid:</span><span class="sxs-lookup"><span data-stu-id="2b987-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="2b987-106">De migratiebatch en -aanvragen moeten binnen enkele minuten worden hervat en voltooid.</span><span class="sxs-lookup"><span data-stu-id="2b987-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

