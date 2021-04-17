---
title: Eigenaar kan geen submap maken door Outlook te gebruiken
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836130"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="512eb-102">Eigenaar kan geen submap maken door Outlook te gebruiken</span><span class="sxs-lookup"><span data-stu-id="512eb-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="512eb-103">**Er is een voortdurend probleem met openbare eigenaren van mappen die submappen maken door Outlook te gebruiken. Het probleem wordt snel opgelost.**</span><span class="sxs-lookup"><span data-stu-id="512eb-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="512eb-104">Ondertussen kunt u een de volgende tijdelijke oplossingen gebruiken:</span><span class="sxs-lookup"><span data-stu-id="512eb-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="512eb-105">Gebruik Outlook voor Mac om submappen te maken, omdat het probleem zich alleen voordoet bij Outlook voor desktop windows (alle versies)</span><span class="sxs-lookup"><span data-stu-id="512eb-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="512eb-106">Laat de beheerder de submap maken door EXO Shell of EAC te gebruiken</span><span class="sxs-lookup"><span data-stu-id="512eb-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="512eb-107">Wijzig DefaultPublicFolderMailbox/EffectivePublicFolderMailbox van de gebruiker naar een ander postvak dan de Inhoud Mailbox voor de map die voor problemen zorgt</span><span class="sxs-lookup"><span data-stu-id="512eb-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="512eb-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="512eb-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="512eb-109">Wacht een uur en start dan outlook cliënt opnieuw op</span><span class="sxs-lookup"><span data-stu-id="512eb-109">Wait for an hour, restart outlook client</span></span>