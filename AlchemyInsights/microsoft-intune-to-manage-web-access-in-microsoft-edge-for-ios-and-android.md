---
title: Microsoft Intune gebruiken om webtoegang te beheren in Microsoft Edge voor iOS en Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989659"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="f0f3f-102">Microsoft Intune gebruiken om webtoegang te beheren in Microsoft Edge voor iOS en Android</span><span class="sxs-lookup"><span data-stu-id="f0f3f-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="f0f3f-103">Met Microsoft Edge voor iOS en Android kan een gebruiker surfen op het web vanuit meerdere, volledig afzonderlijke profielen.</span><span class="sxs-lookup"><span data-stu-id="f0f3f-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="f0f3f-104">De ruimste beveiligingsmogelijkheden voor Microsoft 365-gegevens worden beschikbaar wanneer u zich abonneert op de Enterprise Mobility + Security-suite, die microsoft Intune- en Azure Active Directory Premium-functies bevat, zoals voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="f0f3f-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="f0f3f-105">U wilt minimaal een beleid voor voorwaardelijke toegang implementeren waarmee (1) gebruikers verbinding kunnen maken vanaf mobiele apparaten met Microsoft Edge voor iOS en Android en dat (2) een Microsoft Intune-beleid voor app-beveiliging implementeert dat een beveiligde browse-ervaring biedt.</span><span class="sxs-lookup"><span data-stu-id="f0f3f-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="f0f3f-106">Zie voor meer informatie over hoe u voorwaardelijke toegang en beleid kunt gebruiken:</span><span class="sxs-lookup"><span data-stu-id="f0f3f-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="f0f3f-107">Beleid voor voorwaardelijke toegang van Azure Active Directory toepassen</span><span class="sxs-lookup"><span data-stu-id="f0f3f-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="f0f3f-108">Microsoft Intune-appbeveiligingsbeleid maken</span><span class="sxs-lookup"><span data-stu-id="f0f3f-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="f0f3f-109">Eén aanmelding gebruiken voor met Azure Active Directory verbonden web-apps in met beleid beveiligde browsers</span><span class="sxs-lookup"><span data-stu-id="f0f3f-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="f0f3f-110">App-configuratie gebruiken om de browse-ervaring te beheren</span><span class="sxs-lookup"><span data-stu-id="f0f3f-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="f0f3f-111">Het gebruik van alleen werk- en schoolaccounts toestaan</span><span class="sxs-lookup"><span data-stu-id="f0f3f-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="f0f3f-112">Algemene app-configuratiebeleid implementeren</span><span class="sxs-lookup"><span data-stu-id="f0f3f-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="f0f3f-113">App-configuratiebeleid implementeren voor gegevensbescherming</span><span class="sxs-lookup"><span data-stu-id="f0f3f-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="f0f3f-114">Microsoft Endpoint Manager gebruiken om app-configuratiebeleid te implementeren</span><span class="sxs-lookup"><span data-stu-id="f0f3f-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="f0f3f-115">Zie Microsoft Edge voor iOS en Android gebruiken voor toegang tot beheerde app-logboeken voor meer informatie over het openen van beheerde [app-logboeken.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="f0f3f-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
