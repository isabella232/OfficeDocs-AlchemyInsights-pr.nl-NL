---
title: Problemen met het ontwikkelen van toepassingen met Api's
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974380"
---
# <a name="issues-developing-applications-with-apis"></a>Problemen met het ontwikkelen van toepassingen met Api's

Als u wilt beginnen met de API van Azure Active Directory Graph, raadpleegt u de [introductiehandleiding voor Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) of raadpleegt u de documentatie over de [interactieve Azure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Einde van de ondersteuning voor Azure Active Directory Authentication Library (ADAL) en Azure AD Graph API (AAD-grafiek)**

**Vanaf 30 juni 2020** worden niet langer nieuwe functies toegevoegd aan ADAL en Azure AD Graph. We bieden technische ondersteuning en beveiligingsupdates, maar bieden geen functie-updates meer.

**Vanaf 30 juni 2022** wordt de ondersteuning voor ADAL en Azure AD Graph beëindigd en zal u niet langer technische ondersteuning en beveiligingsupdates bieden.

Apps die gebruikmaken van ADAL op bestaande versie van het besturingssysteem werken na dit moment nog niet, maar krijgen geen technische ondersteuning of beveiligingsupdates.

Apps die gebruikmaken van Azure AD Graph na dit tijdstip, kunnen mogelijk geen antwoorden meer ontvangen van het Azure AD-eindpunt.

**ADAL-migratie**

We raden u aan een update uit te voeren voor de [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), met de meest recente functies en beveiligingsupdates.

Als u Microsoft-apps gebruikt, moet u weten dat Microsoft de toepassing van de einde-ondersteunings deadline zal gebruiken voor het migreren van de toepassingen en om te zorgen dat ze profiteren van de voortdurende beveiliging en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Meer informatie over hoe u apps migreert op een platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Als u meer informatie wilt over het gebruik van ADAL, raden we u aan alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met Isv's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw Tenant bieden.

**Migratie van AAD-grafieken**

Volg voor toepassingen die gebruikmaken van Azure AD Graph onze richtlijnen voor het migreren van [Azure AD Graph-apps naar Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Onze migratie controlelijst biedt een aantekening aan de slag](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. De registratie portal van Azure app toont welke toepassingen gebruikmaken van een AAD-grafiek. We raden u aan om alle broncode van uw apps te controleren en, indien van toepassing, contact op te nemen met Isv's of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle AAD-grafiek gebruik in uw Tenant bieden.
1. Als u wilt dat de app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of de beheerder deze de juiste machtigingen verlenen via een toestemming procedure. De [verwijzing naar machtigingen van Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) bevat de machtigingen die zijn gekoppeld aan elke primaire set Microsoft Graph-api's. Ook biedt u informatie over het gebruik van de machtigingen.
