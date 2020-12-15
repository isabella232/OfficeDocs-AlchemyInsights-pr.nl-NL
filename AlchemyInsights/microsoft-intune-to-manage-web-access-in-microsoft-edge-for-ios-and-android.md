---
title: Microsoft intune gebruiken voor het beheren van Web Access in Microsoft Edge voor iOS en Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/10/2020
ms.locfileid: "49677446"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="bea8b-102">Microsoft intune gebruiken voor het beheren van Web Access in Microsoft Edge voor iOS en Android</span><span class="sxs-lookup"><span data-stu-id="bea8b-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="bea8b-103">Met Microsoft Edge voor iOS en Android kunnen gebruikers in het web zoeken naar meerdere, volledig gescheiden profielen.</span><span class="sxs-lookup"><span data-stu-id="bea8b-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="bea8b-104">De uitgebreide beveiligingsmogelijkheden voor Microsoft 365 gegevens zijn beschikbaar wanneer u zich abonneert op een Enterprise Mobility + beveiligingspakket, waaronder Microsoft intune-en Azure Active Directory Premium-functies, zoals voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="bea8b-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="bea8b-105">U dient ten minste een beleid voor voorwaardelijke toegang toe te passen dat gebruikers van mobiele apparaten kunnen verbinden met Microsoft Edge voor iOS en Android en dat (2) een Microsoft intune-beleid voor app-beveiliging biedt met een beveiligde browser ervaring.</span><span class="sxs-lookup"><span data-stu-id="bea8b-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="bea8b-106">Ga als volgt te werk als u wilt weten hoe u voorwaardelijke toegang en beleidsregels kunt gebruiken:</span><span class="sxs-lookup"><span data-stu-id="bea8b-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="bea8b-107">Azure Active Directory-beleid voor voorwaardelijke toegang toepassen</span><span class="sxs-lookup"><span data-stu-id="bea8b-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="bea8b-108">Beveiligingsbeleid voor Microsoft intune-apps maken</span><span class="sxs-lookup"><span data-stu-id="bea8b-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="bea8b-109">Eenmalige aanmelding gebruiken voor Azure Active Directory-verbonden web apps in beleid-beveiligde browsers</span><span class="sxs-lookup"><span data-stu-id="bea8b-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="bea8b-110">De configuratie van de app gebruiken om de browse ervaring te beheren</span><span class="sxs-lookup"><span data-stu-id="bea8b-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="bea8b-111">Het gebruik van alleen werk-en school accounts toestaan</span><span class="sxs-lookup"><span data-stu-id="bea8b-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="bea8b-112">Algemeen configuratiebeleid voor Apps implementeren</span><span class="sxs-lookup"><span data-stu-id="bea8b-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="bea8b-113">Beleid voor de configuratie van de apps implementeren voor gegevensbeveiliging</span><span class="sxs-lookup"><span data-stu-id="bea8b-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="bea8b-114">Microsoft Endpoint Manager gebruiken om het configuratiebeleid voor apps te implementeren</span><span class="sxs-lookup"><span data-stu-id="bea8b-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="bea8b-115">Als u wilt weten hoe u toegang krijgt tot beheerde app-logboeken, raadpleegt u [Microsoft Edge voor IOS en Android gebruiken voor toegang tot de logboeken van beheerde apps](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="bea8b-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
