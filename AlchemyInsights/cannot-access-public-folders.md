---
title: Geen toegang tot openbare mappen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819507"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="fee55-102">Outlook kan geen verbinding maken met openbare mappen</span><span class="sxs-lookup"><span data-stu-id="fee55-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="fee55-103">Als de toegang tot openbare mappen voor sommige gebruikers niet werkt, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="fee55-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="fee55-104">Maak verbinding met EXO PowerShell en configureer de parameter DefaultPublicFolderMailbox op het gebruikersaccount van het probleem op basis van de parameter voor een werkend gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="fee55-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="fee55-105">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="fee55-105">Example:</span></span>

<span data-ttu-id="fee55-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="fee55-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="fee55-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="fee55-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="fee55-108">Wacht ten minste één uur totdat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="fee55-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="fee55-109">Als het probleem blijft bestaan, volgt u [deze procedure om](https://aka.ms/pfcte) problemen met toegang tot openbare mappen op te lossen met Outlook.</span><span class="sxs-lookup"><span data-stu-id="fee55-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="fee55-110">**Bepalen welke gebruikers toegang hebben tot openbare mappen met Outlook:**</span><span class="sxs-lookup"><span data-stu-id="fee55-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="fee55-111">Gebruik Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true of $false</span><span class="sxs-lookup"><span data-stu-id="fee55-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="fee55-112">$true: Gebruikers toegang verlenen tot openbare mappen in Outlook</span><span class="sxs-lookup"><span data-stu-id="fee55-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="fee55-113">$false: Gebruikerstoegang tot openbare mappen in Outlook voorkomen.</span><span class="sxs-lookup"><span data-stu-id="fee55-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="fee55-114">Dit is de standaardwaarde.</span><span class="sxs-lookup"><span data-stu-id="fee55-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="fee55-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="fee55-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="fee55-116">**Opmerking** Met deze procedure kunnen verbindingen alleen worden uitgevoerd met Outlook-bureaublad voor Windows-clients.</span><span class="sxs-lookup"><span data-stu-id="fee55-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="fee55-117">Een gebruiker kan toegang blijven krijgen tot openbare mappen met OWA of Outlook voor Mac.</span><span class="sxs-lookup"><span data-stu-id="fee55-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="fee55-118">Zie Ondersteuning aankondigen voor gecontroleerde verbindingen met openbare mappen [in Outlook voor meer informatie.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="fee55-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>