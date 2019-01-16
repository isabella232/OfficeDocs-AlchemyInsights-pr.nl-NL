---
title: Postbus van gebruiker omzetten in een gedeeld postvak?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284677"
---
U kunt een postbus van gebruiker alleen converteren naar een gedeeld postvak als de gebruiker een Exchange-licentie heeft. Nadat de postbus is geconverteerd, blijven deze weergeven in de lijst met actieve gebruikers omdat gedeelde postvakken in deze lijst opgenomen. Echter, de geconverteerde postbus wordt ook weergegeven in de lijst gedeelde postbus. 
  
Als u probeert te converteren van een postbus in het Exchange-beheerconsole en de conversie is mislukt, wordt de browsercache en cookies wissen en probeer het opnieuw. Als het nog steeds niet werkt, probeert u de postbus in Exchange Management Shell converteren door met de volgende opdracht:
  
```
Set-Mailbox -Type Shared
```

Meer informatie over postbus is beschikbaar in [een postbus van gebruiker om een gedeeld postvak te converteren](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
