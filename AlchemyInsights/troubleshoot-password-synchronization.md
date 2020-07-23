---
title: Problemen met wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387872"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="17e0f-102">Problemen met wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="17e0f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="17e0f-103">Als u problemen met wachtwoordsynchronisatie wilt oplossen, gebruikt u deze taak voor het oplossen van problemen met AAD Connect om te bepalen waarom wachtwoorden niet worden gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="17e0f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="17e0f-104">Ga om te beginnen naar [Directe synchronisatie beheren.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)</span><span class="sxs-lookup"><span data-stu-id="17e0f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="17e0f-105">Open een nieuwe Windows PowerShell-sessie op uw Azure AD Connect-server en selecteer de optie **Uitvoeren als administrator.**</span><span class="sxs-lookup"><span data-stu-id="17e0f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="17e0f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="17e0f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="17e0f-107">Start de wizard Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="17e0f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="17e0f-108">Ga naar de pagina Extra taken > **Volgende problemen oplossen**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="17e0f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="17e0f-109">Selecteer **Starten** om het menu Probleemoplossing van PowerShell te openen.</span><span class="sxs-lookup"><span data-stu-id="17e0f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="17e0f-110">Selecteer **Wachtwoordsynchronisatie oplossen**.</span><span class="sxs-lookup"><span data-stu-id="17e0f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="17e0f-111">Het probleem is meestal dat een wachtwoord niet wordt gesynchroniseerd voor een specifiek gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="17e0f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="17e0f-112">**Notities** Wachtwoordsynchronisatie mislukt als de laatste succesvolle wachtwoordsynchronisatie enige tijd geleden was.</span><span class="sxs-lookup"><span data-stu-id="17e0f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="17e0f-113">Zie Problemen [met wachtwoordhashsynchronisatie oplossen met Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)voor meer hulp bij het oplossen van wachtwoordsynchronisatie.</span><span class="sxs-lookup"><span data-stu-id="17e0f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>