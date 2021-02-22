---
title: Openbare mappen verbergen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315339"
---
# <a name="hide-public-folders"></a><span data-ttu-id="4d218-102">Openbare mappen verbergen</span><span class="sxs-lookup"><span data-stu-id="4d218-102">Hide public folders</span></span>

<span data-ttu-id="4d218-103">**De volledige structuur van openbare mappen verbergen:**</span><span class="sxs-lookup"><span data-stu-id="4d218-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="4d218-104">Gebruik de stappen in [dit artikel](https://aka.ms/ControlPF) om de volledige structuur van openbare mappen te verbergen voor selectieve of alle gebruikers.</span><span class="sxs-lookup"><span data-stu-id="4d218-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="4d218-105">**Een specifieke openbare map verbergen:**</span><span class="sxs-lookup"><span data-stu-id="4d218-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="4d218-106">Machtigingen toevoegen voor gebruikers die toegang moeten hebben tot de openbare map</span><span class="sxs-lookup"><span data-stu-id="4d218-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="4d218-107">Verwijder de gebruiker **Standaard uit** de **machtigingenlijst:**</span><span class="sxs-lookup"><span data-stu-id="4d218-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
