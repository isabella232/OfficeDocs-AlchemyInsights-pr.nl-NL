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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan geen verbinding maken met openbare mappen

Als de toegang tot openbare mappen voor sommige gebruikers niet werkt, gaat u als volgt te werk:

Maak verbinding met EXO PowerShell en configureer de parameter DefaultPublicFolderMailbox op het gebruikersaccount van het probleem op basis van de parameter voor een werkend gebruikersaccount.

Voorbeeld:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Wacht ten minste één uur totdat de wijziging van kracht wordt.

Als het probleem blijft bestaan, volgt u [deze procedure om](https://aka.ms/pfcte) problemen met toegang tot openbare mappen op te lossen met Outlook.
 
**Bepalen welke gebruikers toegang hebben tot openbare mappen met Outlook:**

1.  Gebruik Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true of $false  
      
    $true: Gebruikers toegang verlenen tot openbare mappen in Outlook  
      
    $false: Gebruikerstoegang tot openbare mappen in Outlook voorkomen. Dit is de standaardwaarde.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Opmerking** Met deze procedure kunnen verbindingen alleen worden uitgevoerd met Outlook-bureaublad voor Windows-clients. Een gebruiker kan toegang blijven krijgen tot openbare mappen met OWA of Outlook voor Mac.
 
Zie Ondersteuning aankondigen voor gecontroleerde verbindingen met openbare mappen [in Outlook voor meer informatie.](https://aka.ms/controlpf)