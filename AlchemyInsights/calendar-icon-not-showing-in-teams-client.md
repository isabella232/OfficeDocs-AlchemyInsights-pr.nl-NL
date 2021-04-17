---
title: Agendapictogram dat niet wordt weergegeven in Teams-client
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819948"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Agendapictogram dat niet wordt weergegeven in Teams-client

Het tabblad Agenda in Teams vereist toegang tot een Exchange-postvak via Exchange-webservices. Het Exchange-postvak kan online of on-premises zijn. Voor online gebruikers die het tabblad Agenda niet zien, controleert u of deze [een licentie hebben voor een Exchange Online-postvak en het postvak is ingeschakeld](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Als de gebruiker een geldig postvak in Exchange Online heeft, maar het tabblad Agenda nog steeds niet wordt weergeven, ondervindt u mogelijk een netwerkprobleem. Gebruik de [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) en voer de **Microsoft Exchange-webservices-connectiviteitstests** uit voor de betrokken gebruiker.

Controleer ten slotte de [Teams-apps app-beleidsinstellingen](https://admin.teams.microsoft.com/policies/app-setup) om er zeker van te zijn dat de Agenda-app niet is verwijderd uit het beleid dat op de gebruiker is toegepast (waarschijnlijk de **Wereldwijd (organisatiebreed standaard)**).

Als uw gebruikers on-premises zijn, moet u controleren of de hybride configuratie in orde is. Gebruik de [Wizard hybride configuratie](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) om problemen op te lossen.

Hou in het achterhoofd dat [Teams Exchange 2016 CU3 of hoger vereist](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
