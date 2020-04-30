---
title: Microvertragingen of beperkingen in Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947834"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Microvertragingen of beperkingen in Exchange Online PowerShell

U ziet mogelijk waarschuwingen of vertragingen van het type 'Micro delay applied' bij het uitvoeren van scripts en cmdlets in Exchange Online. In verband hiermee zijn er twee suggesties:

- U kunt proberen om de [Exchange Online v2 PowerShell-module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) te gebruiken, die cmdlets bevat die zijn gebaseerd op REST API en aanzienlijk beter worden uitgevoerd. Dit kan een geweldige oplossing zijn voor veel Get-cmdlets die vaak worden gebruikt.
- Als u cmdlets wilt gebruiken die nog niet in de v2-module voorkomen, raadpleegt u [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) (PowerShell-cmdlets uitvoeren voor een groot aantal gebruikers in Office 365). Hier wordt uitgelegd hoe u de verwachte limieten met betrekking tot PowerShell-beperking in Exchange Online kunt omzeilen.
