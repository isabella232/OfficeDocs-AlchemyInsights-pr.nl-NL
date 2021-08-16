---
title: Problemen met het integreren van naadloze aanmelding met mijn on-premises apps
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028287"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemen met het integreren van naadloze aanmelding met mijn on-premises apps

Ga als volgt te werk om problemen op te lossen met het integreren van naadloze aanmelding met on-premises toepassingen:

**Aanbevolen stappen**

1. Zie Wachtwoordkluisen voor een enkele aanmelding met toepassingsproxy als u een **on-premises** toepassing wilt [configureren voor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)een enkele aanmelding via toepassingsproxy.
1. **Problemen met toepassingsproxy** oplossen: we raden u aan om te beginnen met het controleren van de probleemstroom, [problemen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)met de foutopsporing van toepassingsproxyconnector om te bepalen of de connectors voor toepassingsproxy correct zijn geconfigureerd. Als u nog steeds problemen hebt met het maken van verbinding met de toepassing, volgt u de stappen voor het oplossen van problemen met toepassingsproxyproblemen [met toepassingsopsporing.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) U kunt [CORS-problemen identificeren](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) met behulp van de volgende hulpprogramma's voor foutopsporing in de browser:
    1. Start de browser en blader naar de web-app.
    1. Druk **op F12** om de foutopsporingsconsole naar boven te halen.
    1. Probeer de transactie te reproduceren en controleer het consolebericht. Een CORS-schending veroorzaakt een consolefout over origin.
    1. Sommige CORS-problemen kunnen niet worden opgelost, bijvoorbeeld wanneer uw app wordt omgeleid naar login.microsoftonline.com om te verifiëren en het toegangs token verloopt. Het CORS-gesprek mislukt vervolgens. Een tijdelijke oplossing voor dit scenario is het verlengen van de levensduur van het toegangs token, om te voorkomen dat het verloopt tijdens de sessie van een gebruiker. Zie [Configureerbare token lifetimes in](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)Microsoft identity platform voor meer informatie over hoe u dit doet.

**Aanbevolen documenten**

- [Een enkele aanmelding configureren voor een toepassingsproxytoepassing](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-aanmelding voor on-premises toepassingen met toepassingsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Problemen met toepassingsproxyproxy Azure Active Directory en oplossen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problemen met beperkte delegatieconfiguraties van Kerberos oplossen voor toepassingsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)