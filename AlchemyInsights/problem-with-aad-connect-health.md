---
title: Probleem met AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481463"
---
# <a name="problem-with-aad-connect-health"></a>Probleem met AAD Connect Health

- Controleer of u gemachtigd bent om de bewerking uit te voeren. Globale beheerders hebben standaard toegang. Daarnaast kunt u toegangsbeheer op basis van rollen gebruiken [om](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registratiemachtigingen te delegeren aan Inzender.
- Zorg ervoor dat de vereiste eindpunten zijn ingeschakeld en niet worden geblokkeerd vanwege de firewall. Zie de vereisten voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- De registratie kan mislukken omdat uitgaande communicatie wordt onderworpen aan SSL-inspectie door de netwerklaag.
- Controleer of u de instellingen voor meldingen voor Azure AD Connect Health hebt gecontroleerd. Controleer de instelling. In [deze handleiding](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vindt u meer informatie over het configureren van de meldingsinstellingen voor statusmeldingen voor Azure AD Connect.
- Zie het synchronisatierapport op objectniveau voor meer informatie over het synchronisatierapport voor AAD Connect Health en over het downloaden [ervan.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Voor het oplossen van problemen met statusmeldingen voor [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) volgt u de gids voor het oplossen van problemen met de statusinformatie van AAD Connect en voor veelgestelde vragen, zie Veelgestelde vragen over de [AAD Connect-statusinstallatie.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
