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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996625"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook geen verbinding maken met openbare mappen

Als de toegang tot openbare mappen voor sommige gebruikers niet werkt, gaat u als volgt te werk:

Verbinding maken naar EXO PowerShell en configureert u de parameter DefaultPublicFolderMailbox op het gebruikersaccount van het probleem, op basis van de parameter voor een werkend gebruikersaccount.

Voorbeeld:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Wacht ten minste één uur totdat de wijziging van kracht wordt.

Als het probleem blijft bestaan, volgt u [deze procedure om](https://aka.ms/pfcte) problemen met de toegang tot openbare mappen op te lossen met Outlook.
 
Bepalen welke gebruikers toegang hebben tot **openbare mappen met Outlook:**

1.  Gebruik Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true of $false  
      
    $true: gebruikers toegang geven tot openbare mappen in Outlook  
      
    $false: gebruikers toegang weigeren tot openbare mappen in Outlook. Dit is de standaardwaarde.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Opmerking** Met deze procedure kunnen verbindingen alleen worden besturingselementen met Outlook bureaublad voor Windows clients. Een gebruiker kan openbare mappen blijven openen met OWA of Outlook voor Mac.
 
Zie Ondersteuning aankondigen voor gecontroleerde verbindingen met openbare mappen [in](https://aka.ms/controlpf)Outlook.