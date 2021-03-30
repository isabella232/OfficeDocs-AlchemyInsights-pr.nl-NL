---
title: Eindpunt-DLP configureren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402412"
---
# <a name="configure-endpoint-dlp"></a>Eindpunt-DLP configureren

Met Microsoft Eindpunt-DLP kunt u de DLP-beveiliging en -controle uitbreiden naar gevoelige informatie op Windows 10-apparaten. Nadat apparaten in gebruik zijn genomen bij apparaatbeheer, kunt u DLP-beleid maken om beschermende acties op items af te dwingen. De Activiteitenverkenner kan worden gebruikt om activiteiten voor gevoelige items te bewaken. Zie [Onboarding van apparaten in apparaatbeheer](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) voor meer informatie.  

Aan de slag met Eindpunt-DLP:

- Zorg ervoor dat u de juiste SKU/abonnementenlicenties hebt. Zie voor meer informatie [SKU/abonnementenlicenties](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Controleer de vereiste machtigingen om apparaatbeheer in te schakelen, toegang te krijgen tot de onboardingpagina of apparaatcontrole in of uit te schakelen. Zie [Machtigingen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions) voor meer informatie.
- Onboard apparaten in Apparaatbeheer door de onboarding-procedure voor apparaten te volgen. Als de optie Device Onboarding (preview) ontbreekt onder M365 Compliance  **Instellingen**, controleert u of u de juiste licentie en machtigingen hebt waarnaar hierboven is verwezen. Zie [Onboarding van apparaten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices) voor meer informatie. 
- Maak DLP-beleid ter bescherming van uw gevoelige items. Zie voor meer informatie [DLP-beleidsscenario's voor eindpunten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Zie [Meer informatie over preventie van gegevensverlies voor Microsoft 365-eindpunten (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about) voor meer informatie.

**Belangrijke stappen voor het verzamelen van gegevens, als ondersteuning nodig is:**

1. MDATP Client Analyzer Preview downloaden vanuit [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Voer het hulpprogramma als beheerder uit vanuit het cmd-venster:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Wanneer u wordt gevraagd het aantal minuten voor het verzamelen van traceringen in te voeren: ", voer het aantal minuten in dat nodig is om het scenario uit te voeren
5. Het scenario uitvoeren

Verzamel de uitvoer van het ZIP-bestand dat aan de ondersteuningsagent moet worden gegeven.
