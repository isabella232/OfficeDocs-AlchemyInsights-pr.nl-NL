---
title: Problemen met Wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 589820c945fb20f00431655f9f53196e740bb38f
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655806"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d25ab-102">Problemen met Wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="d25ab-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d25ab-103">Problemen waar geen wachtwoorden gesynchroniseerd met Azure AD verbinden versie 1.1.614.0 of hoger worden:</span><span class="sxs-lookup"><span data-stu-id="d25ab-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d25ab-104">Open een nieuwe Windows PowerShell-sessie op de server Azure AD verbinding maken met de optie **als Administrator uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="d25ab-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="d25ab-105">**Set uitvoeringsbeleid RemoteSigned** of **onbeperkte Set uitvoeringsbeleid**uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="d25ab-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="d25ab-106">Start de wizard Azure AD verbinden.</span><span class="sxs-lookup"><span data-stu-id="d25ab-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="d25ab-107">Ga naar de \*\* extra taken \*\* Selecteer pagina \*\* oplossen \*\*, en klik op **volgende**.</span><span class="sxs-lookup"><span data-stu-id="d25ab-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="d25ab-108">Klik op de pagina probleemoplossing menu **starten om te beginnen met het oplossen van problemen** in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d25ab-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="d25ab-109">Selecteer in het hoofdmenu **Password Synchronization oplossen**.</span><span class="sxs-lookup"><span data-stu-id="d25ab-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="d25ab-110">Selecteer **Wachtwoordsynchronisatie werkt niet op alle**in de submenu.</span><span class="sxs-lookup"><span data-stu-id="d25ab-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="d25ab-111">**Inzicht in de resultaten van de taak voor het oplossen van problemen**</span><span class="sxs-lookup"><span data-stu-id="d25ab-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d25ab-112">De taak voor het oplossen van problemen worden de volgende controles uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="d25ab-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d25ab-113">Dat de functie wachtwoord synchronisatie is ingeschakeld voor uw huurder Azure AD worden gevalideerd.</span><span class="sxs-lookup"><span data-stu-id="d25ab-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="d25ab-114">Valideert de Azure AD Connect-server is niet in een staging-modus.</span><span class="sxs-lookup"><span data-stu-id="d25ab-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="d25ab-115">Voor elke bestaande op ruimten Active Directory-connector (die overeenkomt met een bestaande Active Directory-forest):</span><span class="sxs-lookup"><span data-stu-id="d25ab-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="d25ab-116">Controleert of de functie wachtwoord synchronisatie is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d25ab-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="d25ab-117">Zoekt u wachtwoord synchronisatiegebeurtenissen heartbeat in de gebeurtenislogboeken van Windows-toepassing.</span><span class="sxs-lookup"><span data-stu-id="d25ab-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="d25ab-118">Voor elk Active Directory-domein in Active Directory-connector op de lokalen:</span><span class="sxs-lookup"><span data-stu-id="d25ab-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="d25ab-119">Wordt gecontroleerd of het domein bereikbaar is vanaf de server verbinden met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d25ab-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="d25ab-120">Wordt gecontroleerd of de Active Directory Domain Services (AD DS) rekeningen die worden gebruikt door Active Directory-connector op de ruimten heeft de juiste gebruikersnaam, wachtwoord en machtigingen vereist voor de synchronisatie van wachtwoorden.</span><span class="sxs-lookup"><span data-stu-id="d25ab-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="d25ab-121">Zie voor meer informatie het wachtwoord synchronisatie oplossen [problemen met Wachtwoordsynchronisatie met Azure AD verbinden synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d25ab-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

