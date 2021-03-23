---
title: Werken met verificatiebibliotheken
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035287"
---
# <a name="working-with-authentication-libraries"></a>Werken met verificatiebibliotheken

Als u het msal-probleem (Microsoft Authentication Library) wilt oplossen, voert u de volgende aanbevolen stappen uit:

1. **Werken met MSAL:** [Verificatiebibliotheken van microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - In dit artikel wordt ondersteuning voor Microsoft Authentication Library voor verschillende toepassingstypen beschreven. Het bevat koppelingen naar bibliotheekbroncode. waar u het pakket voor het project van uw app kunt downloaden; en of de bibliotheek gebruikers aanmelden (verificatie), toegang tot beveiligde web-API's (autorisatie) of beide ondersteunt.

2. **Verificatie oplossen:** MsAL ondersteunt verschillende verificatiestromen voor gebruik in verschillende toepassingsscenario's. Afhankelijk van hoe uw clienttoepassing is gemaakt, kan msal een of meer verificatiestromen gebruiken die worden ondersteund door het Microsoft-identiteitsplatform. Deze stromen kunnen verschillende typen tokens en autorisatiecodes produceren en vereisen verschillende tokens om ze te laten werken.

3. **Toegangstokens:** [Toegangstokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) voor microsoft-identiteitsplatform- Lees hoe uw API de claims in een toegangstoken kan valideren en gebruiken. Alle documentatie in dit artikel, behalve waar vermeld, is alleen van toepassing op tokens die zijn uitgegeven voor API's die u hebt geregistreerd. Het is niet van toepassing op tokens die zijn uitgegeven voor API's van Microsoft en deze tokens kunnen ook niet worden gebruikt om te valideren hoe het Microsoft-identiteitsplatform tokens uitdeelt voor een API die u maakt.

**Einde van ondersteuning voor Azure Active Directory Authentication Library (ADAL)**

- **Vanaf 30 juni 2020** worden er geen nieuwe functies meer toegevoegd aan ADAL en Azure AD Graph. We blijven technische ondersteuning en beveiligingsupdates bieden, maar bieden geen functie-updates meer aan.
- **Vanaf 30 juni 2022** beëindigen we de ondersteuning voor ADAL en Azure AD Graph en bieden we geen technische ondersteuning of beveiligingsupdates meer.
- Apps die ADAL gebruiken voor bestaande besturingssysteemversies blijven na deze tijd werken, maar krijgen geen *technische ondersteuning of beveiligingsupdates.*
- Apps met Azure AD Graph na deze periode ontvangen mogelijk geen antwoorden meer van het Azure AD Graph-eindpunt.

**ADAL-migratie**

- We raden u aan bij te werken naar msal, met de nieuwste functies en beveiligingsupdates.
- Als u Microsoft-apps gebruikt, weet dan dat Microsoft bezig is met het migreren van de apps naar MSAL tegen het einde van de ondersteuningsdeadline, zodat ze profiteren van de voortdurende beveiligings- en functieverbeteringen van MSAL.

1. [Lees de veelgestelde vragen over ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Meer informatie over het migreren van apps per platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Als u na het lezen van de handleiding voor het platform van uw app aanvullende vragen hebt, kunt u een bericht plaatsen op [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) met de tag [azure-ad-adal-deprecation] of een probleem openen in de GitHub-opslagplaats van de bibliotheek. Zie de [sectie Talen en frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) van het **MSAL-overzichtsartikel** voor koppelingen naar de repo van elke bibliotheek.
4. **Als u hulp nodig hebt bij het begrijpen van welke van uw apps ADAL** wordt gebruikt, raden we u aan de broncode van al uw apps te controleren. Indien van toepassing, kunt u contact op met onafhankelijke softwareleveranciers (ISV's) of app-providers. Microsoft-ondersteuning kan u ook een lijst met alle niet-Microsoft ADAL-apps in uw tenant bieden.







