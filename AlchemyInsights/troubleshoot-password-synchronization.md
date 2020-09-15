---
title: Problemen met Wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664921"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e8b29-102">Problemen met Wachtwoordsynchronisatie oplossen</span><span class="sxs-lookup"><span data-stu-id="e8b29-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e8b29-103">Voor het oplossen van problemen met Wachtwoordsynchronisatie, begint u met deze AAD-verbinding voor het oplossen van problemen om te bepalen waarom wachtwoorden niet worden gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="e8b29-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="e8b29-104">Als u wilt beginnen, gaat u naar [directe synchronisatie beheren](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="e8b29-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="e8b29-105">Open een nieuwe Windows PowerShell-sessie op de Azure AD Connect-server en selecteer vervolgens de optie **Run as-beheerder** .</span><span class="sxs-lookup"><span data-stu-id="e8b29-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e8b29-106">Voer Set-ExecutionPolicy RemoteSigned of Set-ExecutionPolicy niet beperkt.</span><span class="sxs-lookup"><span data-stu-id="e8b29-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="e8b29-107">Start de wizard Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e8b29-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e8b29-108">Ga naar de pagina aanvullende taken > **volgende problemen oplossen**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="e8b29-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="e8b29-109">Selecteer **Start** om het menu probleem met PowerShell te openen.</span><span class="sxs-lookup"><span data-stu-id="e8b29-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="e8b29-110">Selecteer **problemen met Wachtwoordsynchronisatie oplossen**.</span><span class="sxs-lookup"><span data-stu-id="e8b29-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="e8b29-111">Het probleem is meestal dat een wachtwoord niet wordt gesynchroniseerd voor een specifiek gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="e8b29-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="e8b29-112">**Info** Wachtwoordsynchronisatie mislukt als de laatste geslaagde Wachtwoordsynchronisatie enige tijd geleden was.</span><span class="sxs-lookup"><span data-stu-id="e8b29-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="e8b29-113">Zie [problemen met wachtwoord hash oplossen met Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synchronisatie voor meer hulp bij het oplossen van Wachtwoordsynchronisatie.</span><span class="sxs-lookup"><span data-stu-id="e8b29-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>