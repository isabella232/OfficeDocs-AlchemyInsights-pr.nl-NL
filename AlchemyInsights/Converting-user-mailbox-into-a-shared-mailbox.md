---
title: Postbus van gebruiker omzetten in een gedeeld postvak?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496394"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Het postvak van een gebruiker naar een gedeelde postbus converteren

U kunt een postbus van gebruiker alleen converteren naar een gedeeld postvak als de gebruiker een Exchange-licentie heeft. Nadat de postbus is geconverteerd, blijven deze weergeven in de lijst met actieve gebruikers omdat gedeelde postvakken in deze lijst opgenomen. Echter, de geconverteerde postbus wordt ook weergegeven in de lijst gedeelde postbus. 
  
Als u probeert te converteren van een postbus in het Exchange-beheerconsole en de conversie is mislukt, wordt de browsercache en cookies wissen en probeer het opnieuw. Als het nog steeds niet werkt, probeert u de postbus in Exchange Management Shell converteren door met de volgende opdracht:
  
```
Set-Mailbox -Type Shared
```

Meer informatie over postbus is beschikbaar in [een postbus van gebruiker om een gedeeld postvak te converteren](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
