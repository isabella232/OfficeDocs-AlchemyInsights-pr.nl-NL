---
title: Problemen met Wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353100"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="101e3-102">Problemen met Wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="101e3-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="101e3-103">Problemen waar geen wachtwoorden gesynchroniseerd met Azure AD verbinden versie 1.1.614.0 of hoger worden:</span><span class="sxs-lookup"><span data-stu-id="101e3-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="101e3-104">Open een nieuwe Windows PowerShell-sessie op de server Azure AD verbinding maken met de optie **als Administrator uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="101e3-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="101e3-105">**Set uitvoeringsbeleid RemoteSigned** of **onbeperkte Set uitvoeringsbeleid**uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="101e3-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="101e3-106">Start de wizard Azure AD verbinden.</span><span class="sxs-lookup"><span data-stu-id="101e3-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="101e3-107">Ga naar de pagina **Meer taken** , **problemen met**selecteren en op **volgende**.</span><span class="sxs-lookup"><span data-stu-id="101e3-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="101e3-108">Klik op de pagina probleemoplossing menu **starten om te beginnen met het oplossen van problemen** in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="101e3-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="101e3-109">Selecteer in het hoofdmenu **Password Synchronization oplossen**.</span><span class="sxs-lookup"><span data-stu-id="101e3-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="101e3-110">Selecteer **Wachtwoordsynchronisatie werkt niet op alle**in de submenu.</span><span class="sxs-lookup"><span data-stu-id="101e3-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="101e3-111">**Inzicht in de resultaten van de taak voor het oplossen van problemen**</span><span class="sxs-lookup"><span data-stu-id="101e3-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="101e3-112">De taak voor het oplossen van problemen worden de volgende controles uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="101e3-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="101e3-113">Dat de functie wachtwoord synchronisatie is ingeschakeld voor uw huurder Azure AD worden gevalideerd.</span><span class="sxs-lookup"><span data-stu-id="101e3-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="101e3-114">Valideert de Azure AD Connect-server is niet in een staging-modus.</span><span class="sxs-lookup"><span data-stu-id="101e3-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="101e3-115">Voor elke bestaande op ruimten Active Directory-connector (die overeenkomt met een bestaande Active Directory-forest):</span><span class="sxs-lookup"><span data-stu-id="101e3-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="101e3-116">Controleert of de functie wachtwoord synchronisatie is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="101e3-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="101e3-117">Zoekt u wachtwoord synchronisatiegebeurtenissen heartbeat in de gebeurtenislogboeken van Windows-toepassing.</span><span class="sxs-lookup"><span data-stu-id="101e3-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="101e3-118">Voor elk Active Directory-domein in Active Directory-connector op de lokalen:</span><span class="sxs-lookup"><span data-stu-id="101e3-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="101e3-119">Wordt gecontroleerd of het domein bereikbaar is vanaf de server verbinden met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="101e3-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="101e3-120">Wordt gecontroleerd of de Active Directory Domain Services (AD DS) rekeningen die worden gebruikt door Active Directory-connector op de ruimten heeft de juiste gebruikersnaam, wachtwoord en machtigingen vereist voor de synchronisatie van wachtwoorden.</span><span class="sxs-lookup"><span data-stu-id="101e3-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="101e3-121">Zie voor meer informatie het wachtwoord synchronisatie oplossen [problemen met Wachtwoordsynchronisatie met Azure AD verbinden synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="101e3-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  