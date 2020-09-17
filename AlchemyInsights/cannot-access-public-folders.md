---
title: Geen toegang tot openbare mappen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812542"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c8a92-102">Er kan geen verbinding worden gemaakt met openbare mappen</span><span class="sxs-lookup"><span data-stu-id="c8a92-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c8a92-103">Als openbare mappen voor gebruikers niet werken, kunt u het volgende proberen:</span><span class="sxs-lookup"><span data-stu-id="c8a92-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="c8a92-104">Maak verbinding met EXO PowerShell en configureer de DefaultPublicFolderMailbox-parameter in het gebruikersaccount van het probleem, zodat het overeenkomt met de parameter van een werkend gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="c8a92-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="c8a92-105">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="c8a92-105">Example:</span></span>

<span data-ttu-id="c8a92-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c8a92-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c8a92-107">Set-mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="c8a92-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c8a92-108">Wacht minimaal één uur voordat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="c8a92-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="c8a92-109">Als het probleem zich blijft voordoen, volgt u [deze procedure](https://aka.ms/pfcte) voor het oplossen van problemen met openbare mappen in Outlook.</span><span class="sxs-lookup"><span data-stu-id="c8a92-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="c8a92-110">**Bepalen welke gebruikers toegang hebben tot openbare mappen met Outlook**:</span><span class="sxs-lookup"><span data-stu-id="c8a92-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="c8a92-111">Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True of $false gebruiken</span><span class="sxs-lookup"><span data-stu-id="c8a92-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="c8a92-112">$true: gebruikers toegang geven tot openbare mappen in Outlook</span><span class="sxs-lookup"><span data-stu-id="c8a92-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="c8a92-113">$false: voorkomen dat gebruikers toegang krijgen tot openbare mappen in Outlook.</span><span class="sxs-lookup"><span data-stu-id="c8a92-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="c8a92-114">Dit is de standaardwaarde.</span><span class="sxs-lookup"><span data-stu-id="c8a92-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="c8a92-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="c8a92-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="c8a92-116">**Opmerking** Met deze procedure kunt u alleen verbindingen beheren met de bureaubladversie van Outlook voor Windows-clients.</span><span class="sxs-lookup"><span data-stu-id="c8a92-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="c8a92-117">Een gebruiker kan blijven toegang krijgen tot openbare mappen met OWA of Outlook voor Mac.</span><span class="sxs-lookup"><span data-stu-id="c8a92-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="c8a92-118">Voor meer informatie raadpleegt [u de ondersteuning voor gecontroleerde verbindingen met openbare mappen in Outlook aangekondigde ondersteuning](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="c8a92-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>