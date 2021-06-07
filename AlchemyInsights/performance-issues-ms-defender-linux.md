---
title: Prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793760"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="7c87e-102">Prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux</span><span class="sxs-lookup"><span data-stu-id="7c87e-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="7c87e-103">In dit artikel wordt u begeleid bij de stappen voor het identificeren van prestatieproblemen voor Microsoft Defender voor Eindpunt op Linux.</span><span class="sxs-lookup"><span data-stu-id="7c87e-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="7c87e-104">Het is belangrijk om eerst te controleren of het probleem dat u ondervindt, is opgelost met de [nieuwste versie.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="7c87e-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="7c87e-105">Zie Prestatieproblemen oplossen voor Microsoft Defender voor Eindpunt op Linux om uw onderzoek [te starten.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="7c87e-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="7c87e-106">Uitsluitingen</span><span class="sxs-lookup"><span data-stu-id="7c87e-106">Exclusions</span></span>

<span data-ttu-id="7c87e-107">Uitsluitingen kunnen helpen om prestatieproblemen te beperken.</span><span class="sxs-lookup"><span data-stu-id="7c87e-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="7c87e-108">Controleer uw uitsluitingen voordat u begint, zodat eventuele extra risico's bekend en gedocumenteerd zijn.</span><span class="sxs-lookup"><span data-stu-id="7c87e-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="7c87e-109">Zie Uitsluitingen [configureren en valideren](/microsoft-365/security/defender-endpoint/linux-exclusions)voor Microsoft Defender voor Eindpunt op Linux voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7c87e-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="7c87e-110">Als u meerdere bestanden & mappen die u wilt uitsluiten en ze allemaal op hetzelfde mountpoint staan, is het mogelijk gemakkelijker om het mountpoint uit te sluiten.</span><span class="sxs-lookup"><span data-stu-id="7c87e-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="7c87e-111">Vanaf release 101.22.80 van februari kunt u een volledig bevestigingspunt uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="7c87e-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="7c87e-112">Als bijvoorbeeld /mnt/back-up een mountpoint is, kunt u /mnt/back-up toevoegen aan de lijst met uitsluiten door deze opdracht uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="7c87e-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="7c87e-113">**Opmerking:** Het toevoegen van uitsluitingen verhoogt het risico dat malware niet wordt gedetecteerd en moet zorgvuldig worden verwerkt en geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="7c87e-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="7c87e-114">Hulp nodig?</span><span class="sxs-lookup"><span data-stu-id="7c87e-114">Need Help?</span></span>

<span data-ttu-id="7c87e-115">Als u u op de meest efficiënte manier wilt helpen, verzamelt u de diagnostische gegevens voordat u een ondersteuningscase opent.</span><span class="sxs-lookup"><span data-stu-id="7c87e-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
