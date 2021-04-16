---
title: Voor migratiebatch openbare mappen met de status CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812459"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Voor migratiebatch openbare mappen met de status CompletedWithErrors

Gebruik de volgende stappen om de batch te voltooien en de grote/slechte items over te slaan: 
1. De overgeslagen items voor migratiebatch goedkeuren:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Gebruik de volgende opdracht om de overgeslagen items voor migratieaanvragen goed te keuren die 'Gesynchroniseerd' zijn, maar niet zijn voltooid:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. De migratiebatch en aanvragen moeten binnen enkele minuten worden hervat en voltooid.

