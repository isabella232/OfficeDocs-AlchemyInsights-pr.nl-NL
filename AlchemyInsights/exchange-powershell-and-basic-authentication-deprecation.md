---
title: Exchange PowerShell en de afschaffing van basisverificatie
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
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813467"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell en de afschaffing van basisverificatie

Als u de meest recente informatie wilt over het maken van verbinding met Exchange Online PowerShell zonder het gebruik van basisverificatie, [gaat u hierheen](https://aka.ms/exops-docs). De Windows PowerShell V2 module gebruikt geen basisverificatie.

Houd er rekening mee dat Basisverificatie nog steeds moet zijn ingeschakeld op uw clientcomputer.
De nieuwe PowerShell V2-module gebruikt moderne verificatie om een verbinding tot stand te brengen voor het inschakelen van alle REST V2-cmdlets. Naast de V2-cmdlets krijgt u ook toegang tot oudere RPS-cmdlets (Remote PowerShell) waarvoor een Remote PowerShell-sessie nodig is. Voor het tot stand brengen van een RPS-sessie op Windows-apparaten moet WinRM BasicAuth zijn ingeschakeld op de clientcomputer, ook al gebruikt de module het mechanisme van moderne verificatie om de service te verifiëren. De WinRM-basisverificatiepijplijn wordt gebruikt voor het transport van tokens van moderne verificatie. Als WinRM-basisverificatie is uitgeschakeld op de clientcomputer blijven de nieuwe V2-cmdlets werken (maar de oudere RPS-cmdlets niet).
