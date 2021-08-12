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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943370"
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
