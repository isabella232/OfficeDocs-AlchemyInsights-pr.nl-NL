---
title: Voor de openbare map Migration batch met de status CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744108"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Voor de openbare map Migration batch met de status CompletedWithErrors

Gebruik de volgende stappen om de batch te voltooien en de grote/beschadigde items over te slaan: 
1. De overgeslagen items goedkeuren in migratie batch:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Met de volgende opdracht kunt u de overgeslagen items goedkeuren bij migratie verzoeken die zijn gesynchroniseerd, maar niet zijn voltooid:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. De migratie batch en aanvragen worden binnen enkele minuten hervat en voltooid.

