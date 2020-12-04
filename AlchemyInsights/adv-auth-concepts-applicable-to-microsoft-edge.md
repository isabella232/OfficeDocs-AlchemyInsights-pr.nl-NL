---
title: Basisprincipes van geavanceerde verificatie voor Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573393"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="c2136-102">Basisprincipes van geavanceerde verificatie voor Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c2136-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="c2136-103">Hieronder vindt u de geavanceerde verificatie basis die van toepassing is op Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="c2136-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="c2136-104">**Proactief verificatie**</span><span class="sxs-lookup"><span data-stu-id="c2136-104">**Proactive Authentication**</span></span>

<span data-ttu-id="c2136-105">Wanneer u het [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -beleid inschakelt, probeert Microsoft Edge aangemelde gebruikers niet te verifiëren via Microsoft-services.</span><span class="sxs-lookup"><span data-stu-id="c2136-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="c2136-106">Met regelmatige tussenpozen wordt een online service gebruikt om te controleren op een bijgewerkt manifest met de configuratie voor de proactieve verificatie.</span><span class="sxs-lookup"><span data-stu-id="c2136-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="c2136-107">Voordelen: proactieve verificatie schakelt verificatie in voor de belangrijkste services, zoals het nieuwe tabblad Office.</span><span class="sxs-lookup"><span data-stu-id="c2136-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="c2136-108">Als Bing ook als zoekprogramma wordt gebruikt, kunt u met proactieve verificatie de prestaties van de adresbalk verbeteren en zoekresultaten met de behoeften van uw bedrijf personaliseren.</span><span class="sxs-lookup"><span data-stu-id="c2136-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="c2136-109">**Windows Hallo CredUI voor NTLM-authenticatie**</span><span class="sxs-lookup"><span data-stu-id="c2136-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="c2136-110">Als eenmalige aanmelding (SSO) niet beschikbaar is wanneer een website probeert zich aan te melden bij de gebruiker via het NTLM-of Negotiate-mechanisme, kan de gebruiker de OS-referenties met de website delen en voldoen aan de gebruikersinterface van de Windows hello-referenties.</span><span class="sxs-lookup"><span data-stu-id="c2136-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="c2136-111">Deze aanmeldings stroom wordt alleen weergegeven in Windows 10 en alleen voor gebruikers die geen EENMALIGe aanmelding krijgen tijdens een NTLM of een Negotiate-uitdaging.</span><span class="sxs-lookup"><span data-stu-id="c2136-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="c2136-112">**Automatisch aanmelden met opgeslagen wachtwoorden**</span><span class="sxs-lookup"><span data-stu-id="c2136-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="c2136-113">Gebruikers die het wachtwoord opslaan in Microsoft Edge kunnen automatisch aanmelden bij websites waarop ze hun referenties hebben opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="c2136-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="c2136-114">Gebruikers kunnen deze functie in-of uitschakelen in edge://settings/passwords en u kunt deze configureren in het [Wachtwoordbeheer](https://go.microsoft.com/fwlink/?linkid=2134622) beleid.</span><span class="sxs-lookup"><span data-stu-id="c2136-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
