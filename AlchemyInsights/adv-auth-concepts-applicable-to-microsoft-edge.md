---
title: Basisprincipes van geavanceerde verificatie voor Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573393"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Basisprincipes van geavanceerde verificatie voor Microsoft Edge

Hieronder vindt u de geavanceerde verificatie basis die van toepassing is op Microsoft Edge:

**Proactief verificatie**

Wanneer u het [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -beleid inschakelt, probeert Microsoft Edge aangemelde gebruikers niet te verifiëren via Microsoft-services. Met regelmatige tussenpozen wordt een online service gebruikt om te controleren op een bijgewerkt manifest met de configuratie voor de proactieve verificatie.

Voordelen: proactieve verificatie schakelt verificatie in voor de belangrijkste services, zoals het nieuwe tabblad Office. Als Bing ook als zoekprogramma wordt gebruikt, kunt u met proactieve verificatie de prestaties van de adresbalk verbeteren en zoekresultaten met de behoeften van uw bedrijf personaliseren.

**Windows Hallo CredUI voor NTLM-authenticatie**

Als eenmalige aanmelding (SSO) niet beschikbaar is wanneer een website probeert zich aan te melden bij de gebruiker via het NTLM-of Negotiate-mechanisme, kan de gebruiker de OS-referenties met de website delen en voldoen aan de gebruikersinterface van de Windows hello-referenties. Deze aanmeldings stroom wordt alleen weergegeven in Windows 10 en alleen voor gebruikers die geen EENMALIGe aanmelding krijgen tijdens een NTLM of een Negotiate-uitdaging.

**Automatisch aanmelden met opgeslagen wachtwoorden**

Gebruikers die het wachtwoord opslaan in Microsoft Edge kunnen automatisch aanmelden bij websites waarop ze hun referenties hebben opgeslagen. Gebruikers kunnen deze functie in-of uitschakelen in edge://settings/passwords en u kunt deze configureren in het [Wachtwoordbeheer](https://go.microsoft.com/fwlink/?linkid=2134622) beleid.
