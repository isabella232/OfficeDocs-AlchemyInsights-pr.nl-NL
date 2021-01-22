---
title: Verbindingsproblemen met eenmalige aanmelding
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935110"
---
# <a name="sso-connection-issues"></a>Verbindingsproblemen met eenmalige aanmelding

1. Volg de [handleiding Snelstart: Configureer eigenschappen voor een toepassingshandleiding](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) om uw toepassing te configureren.
2. Volg de onderstaande [](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) richtlijnen, afhankelijk van de gekozen optie voor een aanmelding bij een toepassing en een optie voor een aanmelding:
    - Als u een **on-premises toepassing** wilt configureren voor een eenpersoonsregistratie op basis van **SAML,** gaat u naar SAML-eenregistratie voor on-premises toepassingen met [toepassingsproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Als u een **cloudtoepassing wilt configureren** voor een een aanmelding via een **wachtwoord,** zie Een wachtwoord [een aanmelding configureren.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Als u een **on-premises toepassing voor** een aanmelding via **toepassingsproxy** wilt configureren, gaat u naar Wachtwoord vaulting voor een eenpersoonsregistratie [met toepassingsproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Problemen met** toepassingsproxy oplossen: we raden u [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)aan te beginnen met het controleren van de probleemoplossingsstroom, problemen met toepassingsproxyconnector opsporen, om te bepalen of de connectors voor toepassingsproxy's correct zijn geconfigureerd. Als u nog steeds problemen hebt met het maken van verbinding met de toepassing, volgt u de stroom voor probleemoplossing in [Toepassingsproxytoepassingsproblemen voor foutopsporing.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) U kunt [CORS-problemen identificeren met](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) behulp van hulpprogramma's voor foutopsporing in de browser:
    - Start de browser en blader naar de web-app.
    - Druk **op F12** om de console foutopsporing weer te maken.
    - Probeer de transactie te reproduceren en bekijk het consolebericht. Bij een CORS-overtreding wordt een consolefout over de origin veroorzaakt.
    - Sommige CORS-problemen kunnen niet worden opgelost, bijvoorbeeld wanneer uw app omgeleid naar login.microsoft.com voor verificatie en het toegang token verloopt. Het CORS-gesprek mislukt dan. Een tijdelijke oplossing voor dit scenario is de levensduur van het toegang token te verlengen om te voorkomen dat het verloopt tijdens een sessie van een gebruiker. Zie de levensduur van [token configureren in het Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)voor meer informatie over hoe u dit doet.
4. Problemen oplossen met een eenpersoonsregistratie op basis van **SAML:** we raden u aan problemen bij het aanmelden bij op [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)gebaseerde apps met een enkele aanmelding te controleren, om de oplossingen te vinden voor de problemen die u waarschijnlijk ondervindt.
5. **Probleemoplossing** bij een eenpersoons aanmelden via een wachtwoord: we raden u aan een een aanmelding op basis van een wachtwoord [in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)te controleren om de oplossingen te vinden voor de problemen die u waarschijnlijk ondervindt.
6. Voor verbindingsproblemen bij het gebruik van een VPN, zie Eenmalige aanmelding [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)via VPN en verbinding Wi-Fi gebruiken.
