---
title: Problemen met referenties
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063626"
---
# <a name="issues-with-credentials"></a>Problemen met referenties

[In het Microsoft-identiteitsplatform en de stroom voor OAuth 2.0-clientreferenties](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) wordt beschreven hoe u rechtstreeks kunt programma's met de OAuth 2.0-clientgegevensstroom.

**Hoe beheer ik het wachtwoord of certificaatreferenties van een toepassing?**

In de Azure CLI kunt u de referenties van [az ad-app](https://docs.microsoft.com/cli/azure/ad/app/credential) gebruiken om het wachtwoord of certificaat van een toepassing te verwijderen, op te nemen in een lijst of opnieuw in te stellen.

**Hoe kunnen mijn gebruikers hun wachtwoorden opnieuw instellen?**

Gebruikers moeten zichzelf [registreren om zelf hun wachtwoord opnieuw in te stellen](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) voordat ze hun wachtwoorden opnieuw kunnen instellen. Wanneer een gebruiker zich heeft geregistreerd, kan deze de instructies in dit artikel volgen om het wachtwoord opnieuw in te stellen: Het wachtwoord van uw werk of [school opnieuw instellen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hoe wijzigen mijn gebruikers hun wachtwoorden?**

Gebruikers kunnen de stappen in dit artikel volgen om hun wachtwoorden te wijzigen: [Uw wachtwoord wijzigen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Ze kunnen ook [app-wachtwoorden beheren voor verificatie in twee stappen.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mijn gebruiker krijgt een foutmelding bij het wijzigen of opnieuw instellen van het wachtwoord**

Deze koppeling geeft informatie over veelvoorkomende problemen die kunnen optreden wanneer een gebruiker zijn of haar wachtwoord opnieuw probeert in te [stellen: Algemene problemen en hun oplossingen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Ik heb problemen met het opnieuw instellen van het wachtwoord van een gebruiker**

- Zorg ervoor dat u bent gemachtigd om wachtwoorden opnieuw in te stellen. *Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.

- Zorg ervoor dat u de licentievereisten begrijpt:

  - Er moet ten minste één licentie zijn toegewezen in uw organisatie:
    - **Alleen cloudgebruikers:** betaalde SKU's voor Office 365 (O365) of Azure AD Basic
    - **Cloud- en/of on-premises** gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
    - Zie licentievereisten voor selfservice voor wachtwoord opnieuw instellen voor Azure AD voor meer informatie over [licentievereisten.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Zoek de gebruiker in Azure AD om het wachtwoord van een gebruiker opnieuw in te stellen. Klik vervolgens op het overzichts blade voor die gebruiker op de knop Wachtwoord opnieuw instellen.

**De knop Wachtwoord opnieuw instellen heeft een grijze kleur**

U bent niet gemachtigd om wachtwoorden van **deze** gebruiker opnieuw in te stellen. *Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.

**Ik zie het wachtwoord niet om het blade opnieuw in te stellen**

U bent niet gemachtigd om wachtwoorden opnieuw in te stellen. *Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.

**Ik zie het on-premises integratie blade niet in wachtwoord opnieuw instellen**

- De on-premises integratie blade wordt alleen weergegeven in hybride omgevingen, wat betekent dat u wachtwoordschrijven gebruikt om on-premises gebruikerswachtwoorden te manipuleren.

- U ziet dit blade niet als:

  - U gebruikt wachtwoordschrijven niet
  - Er is een probleem met de installatie/connectiviteit van wachtwoordopschrijven
  - Er is een probleem met de installatie/connectiviteit van Azure AD Connect
  - Zie Problemen met wachtwoordopschrijven oplossen voor meer stappen voor het oplossen van problemen met [wachtwoordopschrijven.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ik weet niet hoe ik het wachtwoord van een gebruiker opnieuw moet instellen**

1. Meld u aan bij de Azure Portal als een geschikte beheerder.
2. Ga naar de **blade Gebruikers en groepen,** selecteer **Alle gebruikers.**
3. Selecteer een gebruiker in de lijst.
4. Selecteer Voor de geselecteerde gebruiker Overzicht **en** selecteer vervolgens Wachtwoord opnieuw instellen op de **opdrachtbalk.**
5. Selecteer de **knop Wachtwoord opnieuw** instellen en volg de instructies op het scherm.
    - Alleen resets uitgevoerd via de **ondersteuning van Azure Portal** bieden ondersteuning voor wachtwoordschrijven.

**Ik stel het wachtwoord van een on-premises gebruiker opnieuw in vanuit de Office 365-beheerportal of de mobiele Office 365-toepassing, maar de gebruiker kan zich nog steeds niet aanmelden**

Wachtwoord terugschrijven wordt niet ondersteund in deze portal. Stel het wachtwoord van de gebruiker opnieuw in in de Azure Portal.
