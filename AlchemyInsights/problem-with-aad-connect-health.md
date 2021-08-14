---
title: Probleem met AAD Verbinding maken Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923747"
---
# <a name="problem-with-aad-connect-health"></a>Probleem met AAD Verbinding maken Health

- Controleer of u gemachtigd bent om de bewerking uit te voeren. Globale beheerders hebben standaard toegang. Daarnaast kunt u toegangsbeheer [op basis van rollen gebruiken](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) om registratiemachtigingen te delegeren aan Inzender.
- Controleer of de vereiste eindpunten zijn ingeschakeld en niet worden geblokkeerd vanwege de firewall. Zie vereisten voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registratie kan mislukken als gevolg van uitgaande communicatie die wordt onderworpen aan SSL-inspectie door de netwerklaag.
- Controleer of u de meldingsinstellingen voor Azure AD Verbinding maken Health. Controleer uw instelling. In [deze handleiding](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) kunt u begrijpen hoe u de instellingen voor meldingen configureert voor Azure AD Verbinding maken statusmeldingen.
- Zie [Objectniveausynchronisatierapport](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)voor meer Verbinding maken AAD-synchronisatierapport en hoe u dit kunt downloaden.

Als u problemen wilt oplossen met [AAD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Verbinding maken Gezondheidswaarschuwingen, volgt u de handleiding voor probleemoplossing voor AAD Verbinding maken Health data freshness alerts en voor veelgestelde vragen, zie Veelgestelde vragen over [AAD-Verbinding maken](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)Health-installatie.
