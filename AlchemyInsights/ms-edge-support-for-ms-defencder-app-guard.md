---
title: Ondersteuning van Microsoft Edge voor Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583365"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Ondersteuning van Microsoft Edge voor Microsoft Defender Application Guard

Voor Application Guard is ontworpen voor Windows 10 en Microsoft Edge, wordt in Application Guard een hardwarematige, door een gebruiker gebruikgemaakt van een niet-vertrouwde site, van een geïsoleerde, Hyper-V-ingeschakelde container, gescheiden van het host Operating System.

Een beheerder van het bedrijf definieert een lijst met vertrouwde websites, Cloud bronnen en interne netwerken. Wanneer een gebruiker een site bezoekt die niet in de lijst staat, wordt in Microsoft Edge de site in de container geopend. Dit betekent dat als de site schadelijk is voor de hostcomputer, de hostcomputer niet is beveiligd en de kwaadwillende persoon geen toegang krijgt tot de bedrijfsgegevens.

Installatie van extensies in de container wordt ondersteund op Microsoft Edge versie 81 en kan worden beheerd via een beleid. Het updateURL-adres dat wordt gebruikt in het ExtensionInstallForcelist-beleid, moet als een neutrale resource worden toegevoegd aan het netwerkgeïsoleerde beleid dat wordt gebruikt door Application Guard.

Zie [Microsoft edge support voor Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229)voor meer informatie.
