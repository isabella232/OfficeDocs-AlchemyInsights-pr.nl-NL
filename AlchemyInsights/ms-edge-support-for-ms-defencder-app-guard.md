---
title: Ondersteuning van Microsoft Edge voor Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583365"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="41f23-102">Ondersteuning van Microsoft Edge voor Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="41f23-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="41f23-103">Voor Application Guard is ontworpen voor Windows 10 en Microsoft Edge, wordt in Application Guard een hardwarematige, door een gebruiker gebruikgemaakt van een niet-vertrouwde site, van een geïsoleerde, Hyper-V-ingeschakelde container, gescheiden van het host Operating System.</span><span class="sxs-lookup"><span data-stu-id="41f23-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="41f23-104">Een beheerder van het bedrijf definieert een lijst met vertrouwde websites, Cloud bronnen en interne netwerken.</span><span class="sxs-lookup"><span data-stu-id="41f23-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="41f23-105">Wanneer een gebruiker een site bezoekt die niet in de lijst staat, wordt in Microsoft Edge de site in de container geopend.</span><span class="sxs-lookup"><span data-stu-id="41f23-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="41f23-106">Dit betekent dat als de site schadelijk is voor de hostcomputer, de hostcomputer niet is beveiligd en de kwaadwillende persoon geen toegang krijgt tot de bedrijfsgegevens.</span><span class="sxs-lookup"><span data-stu-id="41f23-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="41f23-107">Installatie van extensies in de container wordt ondersteund op Microsoft Edge versie 81 en kan worden beheerd via een beleid.</span><span class="sxs-lookup"><span data-stu-id="41f23-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="41f23-108">Het updateURL-adres dat wordt gebruikt in het ExtensionInstallForcelist-beleid, moet als een neutrale resource worden toegevoegd aan het netwerkgeïsoleerde beleid dat wordt gebruikt door Application Guard.</span><span class="sxs-lookup"><span data-stu-id="41f23-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="41f23-109">Zie [Microsoft edge support voor Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="41f23-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
