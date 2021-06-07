---
title: Webinars Teams inschakelen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793652"
---
# <a name="enable-teams-webinars"></a>Webinars Teams inschakelen

Webinars zijn standaard ingeschakeld. U kunt beheren wie webinars kan plannen en Teams met behulp van Teams PowerShell-opdrachten.

- Alle gebruikers die een vergadering kunnen maken, kunnen ook een webinarvergadering maken. Als u wilt beheren wie de webinars Teams plannen, gebruikt *u AllowMeetingRegistration*. 
- *WhoCanRegister* is standaard ingeschakeld en ingesteld op **Iedereen.** Als u de registratie van vergaderingen wilt uitschakelen, stelt *u AllowMeetingRegistration in* op **Onwaar.**

Als u deze instellingen wilt wijzigen, moet u Teams [PowerShell installeren.](/microsoftteams/teams-powershell-install) Vergaderbeleid wordt ook afgedwongen op Teams webinars. Als anonieme join bijvoorbeeld is uitgeschakeld in vergaderingsinstellingen, kunnen anonieme gebruikers niet deelnemen aan webinars.

Zie Configureren wie zich kan registreren voor webinars voor meer informatie over het configureren van wie zich kan [registreren voor webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Zie Besturingselementinstellingen voor Microsoft-lijsten voor meer informatie over instellingen voor [Microsoft-lijsten.](/sharepoint/control-lists)