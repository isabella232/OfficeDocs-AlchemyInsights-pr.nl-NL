---
title: Een verwijderde openbare map herstellen
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063628"
---
# <a name="restore-a-deleted-public-folder"></a>Een verwijderde openbare map herstellen

**Verwijderde items uit een openbare map herstellen:**

- Zie Verwijderen van verwijderde items niet herstellen uit een openbare map zonder [e-mail in Outlook 2016](https://aka.ms/pfrec).
 
**Een verwijderde openbare map (van welk type dan ook) herstellen:** 

- Gebruik de volgende opdracht EXO PowerShell:

    Syntaxis:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Naam -eq\<" name_of_deleted_public_Folder"}; Pad pad set-PublicFolder \<$pf.identity -Path waar de map wordt hersteld>

    Voorbeeld: met de volgende opdracht herstelt u Submap1 en plaatst u deze onder \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Naam -eq "Submap1"}; Set-PublicFolder $pf.identity -Path \Parent1

Zie [Een verwijderde openbare map herstellen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) voor meer informatie.
