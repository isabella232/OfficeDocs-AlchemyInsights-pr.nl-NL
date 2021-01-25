---
title: Problemen met koppelingen en Url's
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974302"
---
# <a name="issues-with-links-and-urls"></a>Problemen met koppelingen en Url's

Url's omleiden URI/antwoord Url's (beide expressies zijn doorlopend) zijn de Url's die worden gebruikt door het Microsoft-identiteits platform, zodat de door apps gevraagde tokens worden geretourneerd. Zie de volgende artikelen voor meer informatie over deze Url's:

- [Verificatie stromen en toepassings scenario's](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) : informatie over de omleidings uri's in de **app-registratie** pagina voor elk scenario.
- [Url's en beperkingen voor het omleiden van url's/antwoorden](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ik weet niet hoe ik de juiste URL/antwoord-URL voor omleiding voor mijn app Registreer**

Wanneer u zich aanmeldt met de toepassing die u wilt ontwikkelen, wordt in het dialoogvenster Aanmelden AADSTS50011 weergegeven **: de antwoord-URL die in de aanvraag is opgegeven, voldoet <your app ID> niet aan de antwoord-url's die zijn geconfigureerd voor de toepassing**, u moet aan de aanvraag voor de toepassing zijn toegevoegd, de omleidings-URL die door uw code voor de tokenaanvraag voor het Microsoft-

Als u een antwoord-URL wilt toevoegen, gaat u naar het tabblad **verificatie** op de pagina voor het **registreren** van de toepassing in de Azure-Portal en voegt u een vermelding toe in de sectie **uri's omleiden** . Omleidings-Uri's worden getypt (Web of Mobile/Desktop). Welke waarde u moet opgeven, is afhankelijk van het type toepassing dat u maakt, zoals hieronder wordt beschreven:

- Voor toepassingen met een enkele pagina en web-apps is de antwoord-URL een URL in uw toepassing. Zie een toepassing van een [toepassing voor één pagina](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) of [Registreer een web-app-app met behulp van Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Voor desktop-apps: de waarde die u wilt kiezen, is afhankelijk van:
    - het platform (MacOS wijkt af van Windows of Linux)
    - de manier waarop u de token (interactief) met de programmacode stroom verwerft, met geïntegreerde Windows-verificatie [IWA] of met gebruikersnaam/wachtwoord.
    Voor meer informatie raadpleegt u [bureaubladtoepassingen-app-registratie-omleiding van URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Voor mobiele toepassingen is de omleidings-URI afhankelijk van:
    - het platform (iOS/Android/UWP)
    - de gegevens die worden gebruikt voor het maken van de app, zoals de bundel-ID in iOS, en de naam van het pakket en de hash van een handtekening in de registratie van de Azure-Portal-app helpt u. Zie [platform Configuration en redirect uri's](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)voor meer informatie.

> [!NOTE]
> Web-Api's en sommige van de stil methoden voor het verkrijgen van tokens (IWA en gebruikersnaam/wachtwoord) hebben geen omleidings-URI nodig.

**Ik heb mijn webtoepassing geïmplementeerd en als ik de geïmplementeerde app test, krijg ik een bericht dat de URL niet overeenkomt**

U kunt omleidings-Uri's toevoegen voor alle locaties waarop u uw webtoepassing implementeert. Voor meer informatie raadpleegt [u een web-app-app registreren met behulp van Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> U kunt omleidings-URI voor een locatie toevoegen direct nadat u de toepassing op deze locatie hebt geïmplementeerd.

**Ik kan niet voldoende antwoord-Url's registreren**

U bent een ISV en hebt een of meer omleidings-Uri's voor elke klant van uw eigen klant. U wilt migreren van ADAL/Azure AD v 1.0 naar MSAL/the Microsoft Identity platform en u hebt het [maximum aantal omleidings-uri's](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)bereikt. Om dit op te lossen, kunt u [omleid uri's toevoegen aan service-principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) die overeenkomen met elk van uw klanten.
