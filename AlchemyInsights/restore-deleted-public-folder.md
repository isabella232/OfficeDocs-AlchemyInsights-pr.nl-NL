---
title: Een verwijderde openbare map herstellen
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809434"
---
# <a name="restore-a-deleted-public-folder"></a>Een verwijderde openbare map herstellen

**Verwijderde items uit een openbare map herstellen:**

- Zie U kunt verwijderde items niet herstellen uit een openbare map zonder [e-mail in Outlook 2016.](https://aka.ms/pfrec)
 
**Een verwijderde openbare map (van elk type) herstellen:** 

- Gebruik de volgende opdracht EXO PowerShell:

    Syntaxis:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Voorbeeld: Met de volgende opdracht wordt Submap1 hersteld en onder \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Zie [Een verwijderde openbare map herstellen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) voor meer informatie.
