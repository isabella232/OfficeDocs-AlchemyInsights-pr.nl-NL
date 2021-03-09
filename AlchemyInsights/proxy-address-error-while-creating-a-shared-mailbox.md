---
title: Fout met proxyadres bij het maken van een gedeeld postvak
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568285"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Fout met proxyadres bij het maken van een postvak of ander object met e-mail

Als u een object wilt maken dat e-mail kan gebruiken (postvak, gedeeld postvak, enzovoort) en het foutbericht 'Het proxyadres 'SMTP:alias@domain.com' wordt gebruikt...' hebt ontvangen, wordt het gekozen e-mailadres al overgenomen door een ander object in uw organisatie met e-mail.
  
U moet de gebruiker, groep, het gedeelde postvak of de openbare map met dit e-mailadres vinden en deze verwijderen of het e-mailadres wijzigen. Vervolgens kunt u een nieuw object met e-mail maken met het gratis e-mailadres. Gebruik Zoeken op de startpagina om de zoekfunctie te vinden. U kunt ook de volgende PowerShell-opdracht van Exchange Online gebruiken om hier naar te zoeken:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Als u het bestaande e-mailadres niet wilt verwijderen, kiest u een nieuw e-mailadres voor het nieuwe object dat u maakt.
  