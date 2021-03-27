---
title: Geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398552"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="22ad3-102">Geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="22ad3-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="22ad3-103">Hieronder volgen de geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="22ad3-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="22ad3-104">**Proactieve verificatie**</span><span class="sxs-lookup"><span data-stu-id="22ad3-104">**Proactive Authentication**</span></span>

<span data-ttu-id="22ad3-105">Wanneer u het [ProactiveAuthEnabled-beleid](https://go.microsoft.com/fwlink/?linkid=2134621) inschakelen, probeert Microsoft Edge aangemelde gebruikers proactief te verifiëren via Microsoft-services.</span><span class="sxs-lookup"><span data-stu-id="22ad3-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="22ad3-106">Met regelmatige tussenpozen wordt een onlineservice gebruikt om te controleren op een bijgewerkt manifest met de configuratie voor Proactieve verificatie.</span><span class="sxs-lookup"><span data-stu-id="22ad3-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="22ad3-107">Voordelen: Met proactieve verificatie kan verificatie worden gebruikt voor belangrijke services, zoals de nieuwe tabbladpagina van Office.</span><span class="sxs-lookup"><span data-stu-id="22ad3-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="22ad3-108">Als Bing wordt gebruikt als de zoekmachine, verbetert Proactieve verificatie ook de prestaties van de adresbalk en helpt u zoekresultaten te genereren die zijn afgestemd op de behoeften van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="22ad3-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="22ad3-109">**Windows Hello CredUI voor NTLM-verificatie**</span><span class="sxs-lookup"><span data-stu-id="22ad3-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="22ad3-110">Als eenmalige aanmelding (SSO) niet beschikbaar is wanneer een website de gebruiker probeert aan te melden via het mechanisme NTLM of Onderhandelen, kan de gebruiker met deze functie de referenties van het besturingssysteem delen met de website en de verificatie-uitdaging aangaan met behulp van de Windows Hello Cred-gebruikersinterface.</span><span class="sxs-lookup"><span data-stu-id="22ad3-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="22ad3-111">Deze aanmeldingsstroom wordt alleen weergegeven in Windows 10 en alleen voor gebruikers die geen SSO krijgen tijdens een NTLM- of een onderhandelingen-uitdaging.</span><span class="sxs-lookup"><span data-stu-id="22ad3-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="22ad3-112">**Opgeslagen wachtwoorden gebruiken om u automatisch aan te melden**</span><span class="sxs-lookup"><span data-stu-id="22ad3-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="22ad3-113">Gebruikers die wachtwoorden opslaan in Microsoft Edge kunnen automatische aanmelding inschakelen bij websites waar ze referenties hebben opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="22ad3-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="22ad3-114">Gebruikers kunnen deze functie in- of uitschakelen in edge://settings/passwords en u kunt deze configureren in het [beleid voor wachtwoordbeheer.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="22ad3-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
