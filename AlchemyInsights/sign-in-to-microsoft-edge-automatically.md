---
title: Meld u automatisch aan bij Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398724"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="8820e-102">Meld u automatisch aan bij Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8820e-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="8820e-103">Microsoft Edge gebruikt het standaardaccount van het besturingssysteem om automatisch een gebruiker aan te melden op basis van de configuratie van het apparaat van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="8820e-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="8820e-104">De scenario's van elk type apparaatconfiguratie en het afhankelijke aanmeldingsproces van de gebruiker worden hieronder beschreven:</span><span class="sxs-lookup"><span data-stu-id="8820e-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="8820e-105">**Het apparaat is hybride/AAD-J:** Deze optie is beschikbaar in Windows 10, windows op lager niveau en bijbehorende serverversies.</span><span class="sxs-lookup"><span data-stu-id="8820e-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8820e-106">Gebruikers worden automatisch aangemeld met hun Ad-accounts (Azure Active Directory).</span><span class="sxs-lookup"><span data-stu-id="8820e-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="8820e-107">**Het apparaat is domeingevoegd:** deze optie is beschikbaar in Windows 10, windows op lager niveau en bijbehorende serverversies.</span><span class="sxs-lookup"><span data-stu-id="8820e-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8820e-108">Gebruikers met domeinaccounts worden standaard niet automatisch aangemeld. Gebruik het beleid **ConfigureOnPremisesAccountAutoSignIn** om automatische aanmelding voor hen in te stellen.</span><span class="sxs-lookup"><span data-stu-id="8820e-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="8820e-109">Als u automatische aanmelding wilt inschakelen voor gebruikers met Azure AD-accounts, kunt u overwegen om hybride deel te nemen aan hun apparaten.</span><span class="sxs-lookup"><span data-stu-id="8820e-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="8820e-110">Het standaardaccount van het besturingssysteem is een **Microsoft-account:** deze optie is beschikbaar in Windows 10 RS3 (versie 1709, build 10.0.16299) en latere versies.</span><span class="sxs-lookup"><span data-stu-id="8820e-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="8820e-111">Het is onwaarschijnlijk dat het scenario zich op ondernemingsapparaten voordoet.</span><span class="sxs-lookup"><span data-stu-id="8820e-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="8820e-112">Als het standaardaccount van het besturingssysteem echter een Microsoft-account is, wordt de gebruiker automatisch door Microsoft Edge met het Microsoft-account aanmelden.</span><span class="sxs-lookup"><span data-stu-id="8820e-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
