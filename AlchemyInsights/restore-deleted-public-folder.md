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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="32ec0-102">Een verwijderde openbare map herstellen</span><span class="sxs-lookup"><span data-stu-id="32ec0-102">Restore a deleted public folder</span></span>

<span data-ttu-id="32ec0-103">**Verwijderde items uit een openbare map herstellen:**</span><span class="sxs-lookup"><span data-stu-id="32ec0-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="32ec0-104">Zie Verwijderen van verwijderde items niet herstellen uit een openbare map zonder [e-mail in Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="32ec0-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="32ec0-105">**Een verwijderde openbare map (van welk type dan ook) herstellen:**</span><span class="sxs-lookup"><span data-stu-id="32ec0-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="32ec0-106">Gebruik de volgende opdracht EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="32ec0-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="32ec0-107">Syntaxis:</span><span class="sxs-lookup"><span data-stu-id="32ec0-107">Syntax:</span></span>

    ><span data-ttu-id="32ec0-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Naam -eq\<" name_of_deleted_public_Folder"}; Pad pad set-PublicFolder \<$pf.identity -Path waar de map wordt hersteld></span><span class="sxs-lookup"><span data-stu-id="32ec0-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="32ec0-109">Voorbeeld: met de volgende opdracht herstelt u Submap1 en plaatst u deze onder \Parent1:</span><span class="sxs-lookup"><span data-stu-id="32ec0-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="32ec0-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Naam -eq "Submap1"}; Set-PublicFolder $pf.identity -Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="32ec0-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="32ec0-111">Zie [Een verwijderde openbare map herstellen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="32ec0-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
