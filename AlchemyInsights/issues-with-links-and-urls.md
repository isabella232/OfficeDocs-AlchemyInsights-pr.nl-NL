---
title: Problemen met koppelingen en URL's
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707877"
---
# <a name="issues-with-links-and-urls"></a>Problemen met koppelingen en URL's

Redirect URI/reply-URL's (beide uitdrukkingen worden gebruikt) zijn URL's die gebruikt worden door het Microsoft identity platform om tokens die door de app aangevraagd werden terug te geven. Zie de volgende artikelen voor meer informatie:

- [Verificatiestromen en toepassingsscenario's](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios): Informatie over de redirect URI's in de pagina **App-registratie** voor elk scenario.
- [Beperkingen voor URI/reply-URL's](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ik weet niet hoe de juiste redirect URI/reply URL te registreren voor mijn app**

Wanneer je je aanmeldt bij de toepassing die je aan het ontwikkelen bent, moet je, als het aanmeldingsdialoogvenster **AADSTS50011: De reply-url die werd opgegeven in de aanvraag komt niet overeen met de reply url's die zijn geconfigureerd voor de toepassing <your app ID>** wordt weergegeven, de redirect URI toevoegen die gebruikt werd door de code in de token-aanvraag aan het Microsoft identity platform aan de registratie van jouw toepassing.

Voeg een reply URL toe door naar het tabblad **Verificatie** te gaan in de pagina **Registratie van toepassing** in het Azure Portal en voer het in de sectie **Redirect URI's**. De waarde die je moet invoeren hangt af van het type toepassing dat je aan het bouwen bent, zoals beschreven hieronder:

- Voor toepassing van een enkele pagina en web-apps is de reply URL een URL in jouw toepassing. Zie [Registratie van enkele-paginatoepassing](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) of [Een web-app registreren met Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Voor desktop-apps hangt de waarde die je nodig hebt af van:
    - het platform (MacOS verschilt van Windows en Linux)
    - de manier waarop je een token verkrijgt (interactief, met codestroom van apparaat, met geïntegreerde Windows-verificatie [IWA] of met gebruikersnaam/wachtwoord).
    Voor meer informatie, zie [Desktop-apps - app-registratie- redirect URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Voor mobiele toepassingen hangt de URI af van:
    - het platform (iOS/Android/UWP)
    - de informatie die werd gebruikt bij het bouwen van de app, zoals de bundel-id in iOS en de naam van het pakket en handtekening hash op Android. De Azure Portal-appregistratie helpt je hierbij. Voor meer informatie, zie [Platformconfiguratie en redirect URI's](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web API's en enkele stille manieren om tokens te verkrijgen (IWA en gebruikersnaam/wachtwoord) vereisen geen redirect URI.

**Ik heb mijn webtoepassing geïmplementeerd en ik krijg een reply url mismatch-bericht wanneer ik de geïmplementeerde app uitprobeer**

Voeg redirect URI's toe voor alle locaties waarop je de webtoepassing implementeert. Voor meer informatie, zie [Web-app registreren met Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Voeg redirect URI toe aan een locatie van zodra je er de app geïmplementeerd hebt.

**Ik kan niet genoeg reply URL's registreren**

Je bent een Independent Software Vendor en hebt een of meerdere redirect URI's voor elke klant. Je wilt migreren van ADAL/Azure AD v1.0 naar MSAL/Microsoft identity platform en je hebt het [maximum aantal redirect URI's](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) bereikt. Je kan dit oplossen door [Redirect URI's toe te voegen aan service-principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) die overeenkomen met iedere klant.
