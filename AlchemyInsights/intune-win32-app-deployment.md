---
title: Implementatie van de Win32-app intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461793"
---
# <a name="intune-win32-app-deployment"></a>Implementatie van de Win32-app intune

Microsoft intune maakt Win32-toepassingen, met inbegrip van, maar niet beperkt tot MSI en. EXE wordt geïmplementeerd op Windows 10-apparaten. Voor de toepassing van het implementatie mechanisme is de functie voor intune-beheer uitbreidingen vereist. De IME wordt automatisch geïnstalleerd als gevolg van het doel van een PowerShell-script of Win32-Toepassingsimplementatie voor een gebruiker/apparaat.

Er gelden ook een reeks vereisten waaraan moet worden voldaan om Win32-apps te kunnen implementeren, waaronder:

- Ondersteunde platformen: Windows 10 versie 1607 of hoger (Enterprise, Pro en Education-versies).
- Ondersteunde architectuur: x86 en x64.
- Apparaatbeheer: AAD, lid geworden van automatisch ingeschreven berichten (waaronder hybride domein, en Groepsbeleid automatisch ingeschreven).
- Opmaak van toepassingspakket:. **intunewin**  -bestand dat is gemaakt door het [Microsoft Win32-hulpprogramma](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)voor het voorbereiden van inhoud.
- Zien
    - Maximale grootte: 8GB.
    - Niet-ondersteunde architectuur: wapen.

Bekijk het document '[een Win32-app in Microsoft intune toevoegen, toewijzen en controleren](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)voor informatie over deze stappen.

Meer informatie over het oplossen van Toepassingsimplementatie in Windows, waaronder Win32-apps, kunt u bekijken in de volgende documenten:

- [Problemen bij het installeren van apps oplossen](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Problemen met Win32-apps oplossen](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)