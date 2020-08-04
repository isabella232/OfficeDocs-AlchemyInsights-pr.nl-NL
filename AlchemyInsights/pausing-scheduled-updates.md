---
title: Geplande updates onderbreken
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555102"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="a0c18-102">Geplande updates onderbreken</span><span class="sxs-lookup"><span data-stu-id="a0c18-102">Pausing scheduled updates</span></span>

<span data-ttu-id="a0c18-103">Wanneer een pauzeopdracht wordt uitgegeven, verwerken apparaten de opdracht pas de volgende keer dat ze inchecken bij Intune.</span><span class="sxs-lookup"><span data-stu-id="a0c18-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="a0c18-104">Hierdoor kunnen uw apparaten het mogelijk hebben:</span><span class="sxs-lookup"><span data-stu-id="a0c18-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="a0c18-105">Installeerde de geplande updates voorafgaand aan het inchecken.</span><span class="sxs-lookup"><span data-stu-id="a0c18-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="a0c18-106">Bent uitgeschakeld toen u de pauzeopdracht uitgaf.</span><span class="sxs-lookup"><span data-stu-id="a0c18-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="a0c18-107">In dit geval, toen de apparaten werden ingeschakeld, hebben ze mogelijk de geplande updates gedownload en geïnstalleerd voordat ze incheckten.</span><span class="sxs-lookup"><span data-stu-id="a0c18-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>