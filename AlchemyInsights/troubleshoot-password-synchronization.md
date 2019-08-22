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
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533802"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ed759-102">Problemen met Wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="ed759-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ed759-103">Problemen waar geen wachtwoorden gesynchroniseerd met Azure AD verbinden versie 1.1.614.0 of hoger worden:</span><span class="sxs-lookup"><span data-stu-id="ed759-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="ed759-104">Open een nieuwe Windows PowerShell-sessie op de server Azure AD verbinding maken met de optie **als Administrator uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="ed759-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="ed759-105">**Set uitvoeringsbeleid RemoteSigned** of **onbeperkte Set uitvoeringsbeleid**uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="ed759-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="ed759-106">Start de wizard Azure AD verbinden.</span><span class="sxs-lookup"><span data-stu-id="ed759-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="ed759-107">Ga naar de pagina **Meer taken** , **problemen met**selecteren en op **volgende**.</span><span class="sxs-lookup"><span data-stu-id="ed759-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="ed759-108">Klik op de pagina probleemoplossing menu **starten om te beginnen met het oplossen van problemen** in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ed759-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="ed759-109">Selecteer in het hoofdmenu **Password Synchronization oplossen**.</span><span class="sxs-lookup"><span data-stu-id="ed759-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="ed759-110">Selecteer **Wachtwoordsynchronisatie werkt niet op alle**in de submenu.</span><span class="sxs-lookup"><span data-stu-id="ed759-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="ed759-111">**Inzicht in de resultaten van de taak voor het oplossen van problemen**</span><span class="sxs-lookup"><span data-stu-id="ed759-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="ed759-112">De taak voor het oplossen van problemen worden de volgende controles uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="ed759-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="ed759-113">Dat de functie wachtwoord synchronisatie is ingeschakeld voor uw huurder Azure AD worden gevalideerd.</span><span class="sxs-lookup"><span data-stu-id="ed759-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="ed759-114">Valideert de Azure AD Connect-server is niet in een staging-modus.</span><span class="sxs-lookup"><span data-stu-id="ed759-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="ed759-115">Voor elke bestaande op ruimten Active Directory-connector (die overeenkomt met een bestaande Active Directory-forest):</span><span class="sxs-lookup"><span data-stu-id="ed759-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="ed759-116">Controleert of de functie wachtwoord synchronisatie is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="ed759-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="ed759-117">Zoekt u wachtwoord synchronisatiegebeurtenissen heartbeat in de gebeurtenislogboeken van Windows-toepassing.</span><span class="sxs-lookup"><span data-stu-id="ed759-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="ed759-118">Voor elk Active Directory-domein in Active Directory-connector op de lokalen:</span><span class="sxs-lookup"><span data-stu-id="ed759-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="ed759-119">Wordt gecontroleerd of het domein bereikbaar is vanaf de server verbinden met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ed759-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="ed759-120">Wordt gecontroleerd of de Active Directory Domain Services (AD DS) rekeningen die worden gebruikt door Active Directory-connector op de ruimten heeft de juiste gebruikersnaam, wachtwoord en machtigingen vereist voor de synchronisatie van wachtwoorden.</span><span class="sxs-lookup"><span data-stu-id="ed759-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="ed759-121">Zie voor meer informatie het wachtwoord synchronisatie oplossen [problemen met Wachtwoordsynchronisatie met Azure AD verbinden synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ed759-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  