---
title: Webinarregistratie beheren
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793710"
---
# <a name="manage-webinar-registration"></a>Webinarregistratie beheren

U beheert wie zich kan registreren voor Teams webinars met behulp Teams PowerShell-opdrachten. Als u Teams Powershell wilt installeren, [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

*WhoCanRegister* is standaard ingeschakeld en ingesteld op **EveryoneInCompany**. Als u wilt dat iedereen, inclusief anonieme gebruikers, zich kan registreren, moet u het vergaderingsbeleid instellen op **Iedereen** met de powershell-opdracht:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Opmerking:** Als anoniem deelnemen is uitgeschakeld in vergaderingsinstellingen, kunnen anonieme gebruikers niet deelnemen aan webinars. Zie Vergaderingsinstellingen beheren in Microsoft Teams voor meer informatie en deze [instelling in Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Als u de registratie van vergaderingen wilt uitschakelen, stelt *u AllowMeetingRegistration in* op **Onwaar.**

Zie Configureren wie zich kan registreren voor webinars voor meer informatie over het configureren van wie zich kan [registreren voor webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Zie Besturingselementinstellingen voor Microsoft-lijsten voor meer informatie over instellingen voor [Microsoft-lijsten.](/sharepoint/control-lists)
