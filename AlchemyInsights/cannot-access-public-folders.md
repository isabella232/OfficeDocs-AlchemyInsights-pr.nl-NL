---
title: Heeft geen toegang tot openbare mappen
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891744"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan geen verbinding maken met openbare mappen

Als toegang tot openbare mappen voor sommige gebruikers niet werkt, probeert u het volgende:

Maak verbinding met EXO PowerShell en configureer de parameter DefaultPublicFolderMailbox op het probleemgebruikersaccount om de parameter op een werkend gebruikersaccount te matchen.

Voorbeeld:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Wacht ten minste een uur tot de wijziging van kracht wordt.

Als het probleem blijft bestaan, volgt u [deze procedure](https://aka.ms/pfcte) om problemen met de toegang tot openbare mappen op te lossen met Outlook.