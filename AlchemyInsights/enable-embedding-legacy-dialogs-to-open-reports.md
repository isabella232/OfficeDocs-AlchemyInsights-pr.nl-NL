---
title: Schakel verouderde dialogen inbedden in op rapporten te openen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814259"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="eae97-102">Schakel verouderde dialogen inbedden in op rapporten te openen</span><span class="sxs-lookup"><span data-stu-id="eae97-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="eae97-103">**Symptoom**</span><span class="sxs-lookup"><span data-stu-id="eae97-103">**Symptom**</span></span>

<span data-ttu-id="eae97-104">Gebruikers kunnen geen rapporten openen.</span><span class="sxs-lookup"><span data-stu-id="eae97-104">Users are unable to open reports.</span></span> <span data-ttu-id="eae97-105">"Er is iets misgegaan.</span><span class="sxs-lookup"><span data-stu-id="eae97-105">"Something has gone wrong.</span></span> <span data-ttu-id="eae97-106">Controleer technische details voor meer informatie."</span><span class="sxs-lookup"><span data-stu-id="eae97-106">Check technical details for more details."</span></span>

<span data-ttu-id="eae97-107">**Oorzaak**</span><span class="sxs-lookup"><span data-stu-id="eae97-107">**Cause**</span></span>

<span data-ttu-id="eae97-108">Rapporten kunnen niet uploaden in UCI met een fout. "Formulieromschrijving is null of niet omschreven."</span><span class="sxs-lookup"><span data-stu-id="eae97-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="eae97-109">Rapporten in UCI vereisen nog steeds verouderde dialogen, dus moet het systeem van een klant nog steeds *allowlegacydialogsembedding* ingeschakeld hebben.</span><span class="sxs-lookup"><span data-stu-id="eae97-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="eae97-110">**Oplossing**</span><span class="sxs-lookup"><span data-stu-id="eae97-110">**Solution**</span></span>

1. <span data-ttu-id="eae97-111">Ga naar **Instellingen >Administratie > Systeeminstellingen > Algemeen tabblad**.</span><span class="sxs-lookup"><span data-stu-id="eae97-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="eae97-112">Stel "Schakel inbeddeln van bepaalde verouderde dialogen in Unified Interface browser klant" in naar **Ja**.</span><span class="sxs-lookup"><span data-stu-id="eae97-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
