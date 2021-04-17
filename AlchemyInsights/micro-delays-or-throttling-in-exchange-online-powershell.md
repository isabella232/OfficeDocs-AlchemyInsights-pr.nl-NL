---
title: Microvertragingen of beperkingen in Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830028"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Microvertragingen of beperkingen in Exchange Online PowerShell

U ziet mogelijk waarschuwingen of vertragingen van het type 'Micro delay applied' bij het uitvoeren van scripts en cmdlets in Exchange Online. In verband hiermee zijn er twee suggesties:

- U kunt proberen om de [Exchange Online v2 PowerShell-module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) te gebruiken, die cmdlets bevat die zijn gebaseerd op REST API en aanzienlijk beter worden uitgevoerd. Dit kan een geweldige oplossing zijn voor veel Get-cmdlets die vaak worden gebruikt.
- Als u cmdlets wilt gebruiken die nog niet in de v2-module voorkomen, raadpleegt u [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) (PowerShell-cmdlets uitvoeren voor een groot aantal gebruikers in Office 365). Hier wordt uitgelegd hoe u de verwachte limieten met betrekking tot PowerShell-beperking in Exchange Online kunt omzeilen.
