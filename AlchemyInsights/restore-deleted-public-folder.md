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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="87aa6-102">Een verwijderde openbare map herstellen</span><span class="sxs-lookup"><span data-stu-id="87aa6-102">Restore a deleted public folder</span></span>

<span data-ttu-id="87aa6-103">**Verwijderde items in een openbare map terugzetten**:</span><span class="sxs-lookup"><span data-stu-id="87aa6-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="87aa6-104">Zie [voor meer informatie over het herstellen van verwijderde items in een openbare map van niet-mail in Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="87aa6-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="87aa6-105">**Een verwijderde openbare map (van elk type) herstellen**:</span><span class="sxs-lookup"><span data-stu-id="87aa6-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="87aa6-106">Gebruik de volgende EXO PowerShell-opdracht:</span><span class="sxs-lookup"><span data-stu-id="87aa6-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="87aa6-107">Syntaxis</span><span class="sxs-lookup"><span data-stu-id="87aa6-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="87aa6-108">Voorbeeld: met de volgende opdracht herstelt u Subfolder1 en plaatst u deze onder \Parent1:</span><span class="sxs-lookup"><span data-stu-id="87aa6-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="87aa6-109">Zie [een verwijderde openbare map herstellen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="87aa6-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
