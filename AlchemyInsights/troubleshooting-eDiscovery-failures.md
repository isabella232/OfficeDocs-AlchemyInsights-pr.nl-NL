---
title: 1490-problemen oplossen-eDiscovery-fouten
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277841"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="08f83-102">Problemen met zoeken in inhoud oplossen</span><span class="sxs-lookup"><span data-stu-id="08f83-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="08f83-103">Ondervindt u problemen met het zoeken van inhoud of het verkrijgen van fouten wanneer u zoekresultaten exporteert?</span><span class="sxs-lookup"><span data-stu-id="08f83-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="08f83-104">U ontvangt bijvoorbeeld het volgende wanneer u zoekopdrachten uitvoert?</span><span class="sxs-lookup"><span data-stu-id="08f83-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="08f83-105">CS008-of CS012-fouten</span><span class="sxs-lookup"><span data-stu-id="08f83-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="08f83-106">Beschikbaarheidsinfo Server-fouten</span><span class="sxs-lookup"><span data-stu-id="08f83-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="08f83-107">Toepassingsfout opgetreden</span><span class="sxs-lookup"><span data-stu-id="08f83-107">Application error occurred</span></span>

<span data-ttu-id="08f83-108">Of bij het zoeken naar en exporteren van resultaten uit een groot aantal postvakken (meer dan 100.000 postvakken), krijgt u een exportfout?</span><span class="sxs-lookup"><span data-stu-id="08f83-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="08f83-109">Voor dit soort fouten probeert u het zoeken naar de inhoudslocaties die mislukt zijn.</span><span class="sxs-lookup"><span data-stu-id="08f83-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="08f83-110">Zie  [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="08f83-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="08f83-111">Als u meer dan een afgesloten 100k postvakken exporteert, moet u de volgende PowerShell gebruiken om de export resultaten te downloaden:  [resultaten uit meer dan afgesloten 100k postvakken exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="08f83-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
