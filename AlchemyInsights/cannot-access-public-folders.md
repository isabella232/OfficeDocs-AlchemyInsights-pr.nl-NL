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
# <a name="outlook-cannot-connect-to-public-folders"></a>Er kan geen verbinding worden gemaakt met openbare mappen

Als openbare mappen voor gebruikers niet werken, kunt u het volgende proberen:

Maak verbinding met EXO PowerShell en configureer de DefaultPublicFolderMailbox-parameter in het gebruikersaccount van het probleem, zodat het overeenkomt met de parameter van een werkend gebruikersaccount.

Voorbeeld:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Wacht minimaal één uur voordat de wijziging van kracht wordt.

Als het probleem zich blijft voordoen, volgt u [deze procedure](https://aka.ms/pfcte) voor het oplossen van problemen met openbare mappen in Outlook.
 
**Bepalen welke gebruikers toegang hebben tot openbare mappen met Outlook**:

1.  Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True of $false gebruiken  
      
    $true: gebruikers toegang geven tot openbare mappen in Outlook  
      
    $false: voorkomen dat gebruikers toegang krijgen tot openbare mappen in Outlook. Dit is de standaardwaarde.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Opmerking** Met deze procedure kunt u alleen verbindingen beheren met de bureaubladversie van Outlook voor Windows-clients. Een gebruiker kan blijven toegang krijgen tot openbare mappen met OWA of Outlook voor Mac.
 
Voor meer informatie raadpleegt [u de ondersteuning voor gecontroleerde verbindingen met openbare mappen in Outlook aangekondigde ondersteuning](https://aka.ms/controlpf).