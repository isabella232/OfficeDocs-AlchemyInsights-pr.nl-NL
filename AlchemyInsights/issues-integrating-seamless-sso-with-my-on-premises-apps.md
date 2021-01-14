---
title: Problemen met het integreren van naadloze SSO met mijn on-premises apps
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868674"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemen met het integreren van naadloze SSO met mijn on-premises apps

Ga als volgt te werk om problemen op te lossen met het integreren van naadloze SSO met on-premises toepassingen:

**Aanbevolen stappen**

1. Als u een **on-premises toepassing** wilt configureren voor **eenmalige aanmelding via toepassingsproxy**, raadpleegt u [wachtwoord kluizen voor eenmalige aanmelding met toepassingsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Problemen met toepassingsproxy oplossen**: u wordt aangeraden om te beginnen met het controleren van de werkstroom voor probleemoplossing, [Foutopsporingsberichten](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) Als u nog steeds problemen ondervindt bij het maken van verbinding met de toepassing, volgt u de stappen voor het oplossen van problemen met de [toepassings proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)van de toepassing. U kunt [CORS-problemen identificeren](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) met behulp van de volgende hulpprogramma's voor foutopsporing in de browser:
    1. Start de browser en blader naar de web-app.
    1. Druk op **F12** om de console foutopsporing te openen.
    1. Probeer de transactie te reproduceren en controleer het consolebericht. Een fout met een CORS veroorzaakt een console fout over origin.
    1. U kunt sommige CORS-problemen niet verhelpen, bijvoorbeeld wanneer uw app wordt omgeleid naar login.microsoftonline.com om te verifiëren, en het toegangstoken verloopt. De CORS-oproep mislukt. Een tijdelijke oplossing voor dit scenario is het verlengen van de levensduur van toegangstokens om te voorkomen dat deze verloopt tijdens de sessie van een gebruiker. Voor meer informatie over hoe u dit doet, raadpleegt u de [levensduur van configureerbare tokens in Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Aanbevolen documenten**

- [Eenmalige aanmelding configureren voor een toepassing voor toepassings proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Eenmalige aanmelding voor SSO voor lokale toepassingen met toepassings proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Meer informatie over CORS en oplossing voor Azure Active Directory Application proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problemen met Kerberos-beperkte delegerings configuraties voor toepassings proxy oplossen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)