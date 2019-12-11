---
title: Geen toegang tot openbare mappen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959490"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan geen verbinding maken met openbare mappen

Als de toegang tot openbare mappen niet voor enkele gebruikers werkt, probeert u het volgende:

Maak verbinding met EXO PowerShell en configureer de DefaultPublicFolderMailbox op het probleem gebruikersaccount zodat deze overeenkomt met een in een werkend gebruikersaccount.

Voorbeeld:

Get-Mailbox Workinggebruiker | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-mailbox ProblemUser-DefaultPublicFolderMailbox \<waarde van de vorige opdracht>

Wacht ten minste één uur voordat de wijziging van kracht wordt.