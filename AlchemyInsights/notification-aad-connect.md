---
title: Melding AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035431"
---
# <a name="notification-aad-connect"></a>Melding AAD Connect

- Controleer of u gemachtigd bent om de bewerking uit te voeren. Globale beheerders hebben standaard toegang. Daarnaast kunt u toegangsbeheer [op basis van rollen gebruiken](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) om registratiemachtigingen te delegeren aan Inzender.
- Controleer of de vereiste eindpunten zijn ingeschakeld en niet worden geblokkeerd vanwege de firewall. Zie vereisten voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registratie kan mislukken als gevolg van uitgaande communicatie die wordt onderworpen aan SSL-inspectie door de netwerklaag.
- Controleer of u de meldingsinstellingen voor Azure AD Connect Health hebt geverifieerd en controleer uw instelling. Zie deze handleiding voor meer informatie over het configureren van de meldingsinstellingen voor Azure AD Connect [Health-meldingen.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Zie Synchronisatierapport op objectniveau voor meer informatie over het synchronisatierapport AAD Connect Health en hoe u het [downloadt.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Als u problemen met AAD Connect Health Alerts wilt oplossen, volgt u de handleiding voor probleemoplossing voor [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) data freshness alerts en voor veelgestelde vragen, zie Veelgestelde [AAD Connect Health-installatievragen.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
