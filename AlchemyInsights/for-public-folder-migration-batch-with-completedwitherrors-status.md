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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043579"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Voor de migratiebatch Openbare map met de status Voltooid met fouten

Gebruik de volgende stappen om de batch te voltooien en sla de grote/slechte items over: 
1. De overgeslagen items op de migratiebatch goedkeuren:

    Batchnaam set-migrationbatch> \<-Overgeslagen artikelen goedkeuren 
2. Gebruik de volgende opdracht om de overgeslagen items op migratieverzoeken goed te keuren die zijn 'Gesynchroniseerd' maar niet zijn voltooid:

    $pf=Get-PublicFolderMailboxMigrationRequest | Word-publicfolderPostvakMigrationRequeststatistics -IncludeReport; ForEach ($i in $pf) {als ($i.LargeItemsEncountered -gt 0 -of $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkipdItemApprovalTime $([DateTime]::UtcNow)}}
3. De migratiebatch en -aanvragen moeten binnen enkele minuten worden hervat en voltooid.

