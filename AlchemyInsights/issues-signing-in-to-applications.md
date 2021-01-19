---
title: Problemen bij het aanmelden bij toepassingen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900874"
---
# <a name="issues-signing-in-to-applications"></a>Problemen bij het aanmelden bij toepassingen

Voer de volgende stappen uit om de oorzaak te bepalen of problemen met de gebruikersaanmelding op te sporen.

1. Start de [Diagnostische aanmelding](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Zoek de gebeurtenis die u wilt analyseren door de details in te voeren voor de gebruiker, toepassing, tijdstip van aanmelden, aanvraag-id of correlatie-id.
3. Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u moet uitvoeren om wijzigingen aan te brengen, indien nodig wijzigingen.

Hier volgen enkele veelvoorkomende problemen die u mogelijk ondervindt bij het aanmelden bij toepassingen:

1. U of de gebruiker **een Azure AD-aanmelding heeft voltooid, maar er verschijnt een onverwachte aanwijzing** -Zie de artikelen [onverwachte toestemming vragen wanneer u zich aanmeldt bij een toepassing](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) en [een onverwachte fout bij het uitvoeren van toestemming voor een toepassing](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. U of een gebruiker **heeft rechtstreeks een toepassing aangemeld bij een toepassing, maar kan zich niet aanmelden bij een deeplink op de aangepaste portal of het toegangsvenster**: Zie problemen oplossen bij het [Aanmelden bij een toepassing vanuit Azure AD mijn apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. U of een gebruiker **heeft een Azure AD-aanmelding voltooid, maar in de toepassing wordt een foutbericht weergegeven en de gebruiker kan de aanmeldings stroom niet voltooien**: het probleem is dat de app het antwoord dat in azure AD is uitgegeven, niet heeft geaccepteerd. Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) om problemen op te lossen.
4. U of een gebruiker **kan zich niet aanmelden bij een niet-galerie programma dat is geconfigureerd voor eenmalige aanmelding voor eenmalige aanmelding**: Volg de instructies in [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) om problemen op te lossen.
5. U of een gebruiker **kan zich niet aanmelden bij een Azure AD-galerie toepassing die voor eenmalig wachtwoord is geconfigureerd**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) om problemen op te lossen.
6. U of een gebruiker **kan zich niet aanmelden bij een Microsoft-toepassing**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) om problemen op te lossen.
7. U of een gebruiker **kan zich niet aanmelden bij een niet-galerie programma dat is geconfigureerd voor federatieve eenmalige aanmelding**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) om problemen op te lossen.
8. U of een gebruiker **kan zich niet aanmelden bij een Azure AD-galerie toepassing die voor federatieve eenmalige aanmelding is geconfigureerd**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) om problemen op te lossen.
9. U of een gebruiker **kan zich niet aanmelden bij een aangepaste toepassing**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) om problemen op te lossen.
10. U of een gebruiker **kan zich niet aanmelden bij een on-premises toepassing met de Azure AD-toepassingsproxy**: Volg [deze stappen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) om problemen op te lossen.

