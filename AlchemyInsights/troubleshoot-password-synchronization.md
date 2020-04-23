---
title: Problemen met wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732505"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="16518-102">Problemen met wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="16518-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="16518-103">Problemen oplossen waarbij geen wachtwoorden worden gesynchroniseerd met Azure AD Connect-versie 1.1.614.0 of hoger:</span><span class="sxs-lookup"><span data-stu-id="16518-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="16518-104">Open een nieuwe Windows PowerShell-sessie op uw Azure AD Connect-server met de optie **Uitvoeren als administrator.**</span><span class="sxs-lookup"><span data-stu-id="16518-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="16518-105">**Uitvoeren Set-ExecutionPolicy RemoteSigned** of **Set-ExecutionPolicy onbeperkt**uitvoeren .</span><span class="sxs-lookup"><span data-stu-id="16518-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="16518-106">Start de wizard Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="16518-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="16518-107">Navigeer naar de pagina **Extra taken,** selecteer **Problemen oplossen**en klik op **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="16518-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="16518-108">Klik op de pagina Probleemoplossing op Starten om het menu probleemoplossing in PowerShell **te starten.**</span><span class="sxs-lookup"><span data-stu-id="16518-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="16518-109">Selecteer in het hoofdmenu **Problemen met wachtwoordsynchronisatie oplossen**.</span><span class="sxs-lookup"><span data-stu-id="16518-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="16518-110">Selecteer **Wachtwoordsynchronisatie werkt helemaal niet in**het submenu.</span><span class="sxs-lookup"><span data-stu-id="16518-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="16518-111">**De resultaten van de probleemoplossingstaak begrijpen**</span><span class="sxs-lookup"><span data-stu-id="16518-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="16518-112">De taak voor het oplossen van problemen voert de volgende controles uit:</span><span class="sxs-lookup"><span data-stu-id="16518-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="16518-113">Valideert dat de functie voor wachtwoordsynchronisatie is ingeschakeld voor uw Azure AD-tenant.</span><span class="sxs-lookup"><span data-stu-id="16518-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="16518-114">Valideert dat de Azure AD Connect-server zich niet in de faseringsmodus bevindt.</span><span class="sxs-lookup"><span data-stu-id="16518-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="16518-115">Voor elke bestaande on-premises Active Directory-connector (die overeenkomt met een bestaand Active Directory-forest):</span><span class="sxs-lookup"><span data-stu-id="16518-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="16518-116">Hiermee wordt gevalideerd dat de functie wachtwoordsynchronisatie is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="16518-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="16518-117">Hiermee wordt gezocht naar heartbeatgebeurtenissen voor wachtwoordsynchronisatie in de logboeken van Windows Application Event.</span><span class="sxs-lookup"><span data-stu-id="16518-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="16518-118">Voor elk Active Directory-domein onder de on-premises Active Directory-connector:</span><span class="sxs-lookup"><span data-stu-id="16518-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="16518-119">Valideert dat het domein bereikbaar is vanaf de Azure AD Connect-server.</span><span class="sxs-lookup"><span data-stu-id="16518-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="16518-120">Hiermee wordt gevalideerd dat de AD DS-accounts (Active Directory Domain Services) die worden gebruikt door de on-premises Active Directory-connector de juiste gebruikersnaam, wachtwoord en machtigingen hebben die nodig zijn voor wachtwoordsynchronisatie.</span><span class="sxs-lookup"><span data-stu-id="16518-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="16518-121">Zie [Wachtwoordsynchronisatie oplossen met Azure AD Connect-synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)voor meer hulp bij het oplossen van problemen met wachtwoordsynchronisatie.</span><span class="sxs-lookup"><span data-stu-id="16518-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  