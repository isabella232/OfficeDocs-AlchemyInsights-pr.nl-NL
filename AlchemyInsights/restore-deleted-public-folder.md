---
title: Een verwijderde openbare map herstellen
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774526"
---
# <a name="restore-a-deleted-public-folder"></a>Een verwijderde openbare map herstellen

**Verwijderde items in een openbare map terugzetten**:

- Zie [voor meer informatie over het herstellen van verwijderde items in een openbare map van niet-mail in Outlook 2016](https://aka.ms/pfrec).
 
**Een verwijderde openbare map (van elk type) herstellen**: 

- Gebruik de volgende EXO PowerShell-opdracht:

    Syntaxis

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Voorbeeld: met de volgende opdracht herstelt u Subfolder1 en plaatst u deze onder \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Zie [een verwijderde openbare map herstellen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) voor meer informatie.
