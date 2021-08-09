---
title: Geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: Auto
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934360"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge

Hieronder volgen de geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge:

**Proactieve verificatie**

Wanneer u het [ProactiveAuthEnabled-beleid](https://go.microsoft.com/fwlink/?linkid=2134621) inschakelen, wordt Microsoft Edge aangemelde gebruikers proactief geverifieerd via Microsoft-services. Met regelmatige tussenpozen wordt een onlineservice gebruikt om te controleren op een bijgewerkt manifest met de configuratie voor Proactieve verificatie.

Voordelen: Met proactieve verificatie kan verificatie worden gebruikt voor belangrijke services, zoals de Office nieuwe tabbladpagina. Als de Bing wordt gebruikt als de zoekmachine, verbetert Proactieve verificatie de prestaties van de adresbalk en helpt u zoekresultaten te genereren die zijn afgestemd op de behoeften van uw bedrijf.

**Windows Hello CredUI voor NTLM-verificatie**

Als eenmalige aanmelding (SSO) niet beschikbaar is wanneer een website de gebruiker probeert aan te melden via het mechanisme NTLM of Onderhandelen, kan de gebruiker met deze functie de besturingssysteemreferenties delen met de website en de verificatie-uitdaging aangaan met behulp van Windows Hello Cred UI. Deze aanmeldingsstroom wordt alleen weergegeven in Windows 10 en alleen voor gebruikers die geen SSO krijgen tijdens een NTLM- of Onderhandelingen-uitdaging.

**Opgeslagen wachtwoorden gebruiken om u automatisch aan te melden**

Gebruikers die wachtwoorden opslaan in Microsoft Edge kunnen automatische aanmelding inschakelen bij websites waar ze referenties hebben opgeslagen. Gebruikers kunnen deze functie in- of uitschakelen in edge://settings/passwords en u kunt deze configureren in het [beleid voor wachtwoordbeheer.](https://go.microsoft.com/fwlink/?linkid=2134622)
