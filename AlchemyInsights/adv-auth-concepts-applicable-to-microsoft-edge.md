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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398552"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge

Hieronder volgen de geavanceerde verificatieconcepten die van toepassing zijn op Microsoft Edge:

**Proactieve verificatie**

Wanneer u het [ProactiveAuthEnabled-beleid](https://go.microsoft.com/fwlink/?linkid=2134621) inschakelen, probeert Microsoft Edge aangemelde gebruikers proactief te verifiëren via Microsoft-services. Met regelmatige tussenpozen wordt een onlineservice gebruikt om te controleren op een bijgewerkt manifest met de configuratie voor Proactieve verificatie.

Voordelen: Met proactieve verificatie kan verificatie worden gebruikt voor belangrijke services, zoals de nieuwe tabbladpagina van Office. Als Bing wordt gebruikt als de zoekmachine, verbetert Proactieve verificatie ook de prestaties van de adresbalk en helpt u zoekresultaten te genereren die zijn afgestemd op de behoeften van uw bedrijf.

**Windows Hello CredUI voor NTLM-verificatie**

Als eenmalige aanmelding (SSO) niet beschikbaar is wanneer een website de gebruiker probeert aan te melden via het mechanisme NTLM of Onderhandelen, kan de gebruiker met deze functie de referenties van het besturingssysteem delen met de website en de verificatie-uitdaging aangaan met behulp van de Windows Hello Cred-gebruikersinterface. Deze aanmeldingsstroom wordt alleen weergegeven in Windows 10 en alleen voor gebruikers die geen SSO krijgen tijdens een NTLM- of een onderhandelingen-uitdaging.

**Opgeslagen wachtwoorden gebruiken om u automatisch aan te melden**

Gebruikers die wachtwoorden opslaan in Microsoft Edge kunnen automatische aanmelding inschakelen bij websites waar ze referenties hebben opgeslagen. Gebruikers kunnen deze functie in- of uitschakelen in edge://settings/passwords en u kunt deze configureren in het [beleid voor wachtwoordbeheer.](https://go.microsoft.com/fwlink/?linkid=2134622)
