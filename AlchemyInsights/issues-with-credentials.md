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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986814"
---
# <a name="issues-with-credentials"></a>Problemen met referenties

Microsoft identity platform en de [OAuth 2.0-clientreferentiesstroom](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) wordt beschreven hoe u rechtstreeks kunt programmeren met de OAuth 2.0-clientreferenties.

**Hoe beheer ik het wachtwoord of de certificaatreferenties van een toepassing?**

In de Azure CLI kunt u de aanmeldingsreferentie voor [az-ad-apps](https://docs.microsoft.com/cli/azure/ad/app/credential) gebruiken om het wachtwoord of certificaatreferenties van een toepassing te verwijderen, te lijsteren of opnieuw in te stellen.

**Hoe stellen mijn gebruikers hun wachtwoorden opnieuw in?**

Gebruikers moeten zich registreren voor het opnieuw instellen van een [selfservicewachtwoord](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) voordat ze hun wachtwoorden opnieuw kunnen instellen. Wanneer een gebruiker zich heeft geregistreerd, kan deze de instructies in dit artikel volgen om het wachtwoord opnieuw in te stellen: Uw werk- of [schoolwachtwoord opnieuw instellen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hoe wijzigen mijn gebruikers hun wachtwoorden?**

Gebruikers kunnen de stappen in dit artikel volgen om hun wachtwoorden te wijzigen: [Uw wachtwoord wijzigen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Ze kunnen ook [app-wachtwoorden beheren voor verificatie in twee stappen.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mijn gebruiker krijgt een foutmelding bij het wijzigen of opnieuw instellen van zijn of haar wachtwoord**

Deze koppeling geeft informatie over veelvoorkomende problemen die kunnen optreden wanneer een gebruiker zijn wachtwoord opnieuw probeert in te stellen: [Veelvoorkomende problemen en hun oplossingen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Ik heb een probleem met het opnieuw instellen van het wachtwoord van een gebruiker**

- Zorg ervoor dat u gemachtigd bent wachtwoorden opnieuw in te stellen. *Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.

- Zorg ervoor dat u de licentievereisten begrijpt:

  - U moet ten minste één licentie hebben toegewezen in uw organisatie:
    - **Alleen gebruikers in de** cloud: betaalde Office 365 (O365) of Azure AD Basic
    - **Cloud- en/of on-premises** gebruikers - Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
    - Zie Licentievereisten voor [selfservicewachtwoord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)opnieuw instellen voor Azure AD voor meer informatie over licentievereisten.
- Als u het wachtwoord van een gebruiker opnieuw wilt instellen, gaat u naar de gebruiker in Azure AD. Klik vervolgens op het overzichtsblad voor die gebruiker op de knop Wachtwoord opnieuw instellen.

**De knop Wachtwoord opnieuw instellen is grijs**

U bent niet gemachtigd om de **wachtwoorden** van deze gebruiker opnieuw in te stellen. *Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.

**Ik zie het wachtwoord voor het opnieuw instellen van het mes niet**

U bent niet gemachtigd wachtwoorden opnieuw in te stellen. *Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen.* Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.

**Ik zie het on-premises integratieblad niet in het opnieuw instellen van wachtwoorden**

- Het on-premises integratieblad wordt alleen weergegeven in hybride omgevingen, wat betekent dat u wachtwoord writeback gebruikt om de wachtwoorden van on-premises gebruikers te manipuleren.

- U ziet dit blad niet als:

  - U gebruikt geen wachtwoord writeback
  - Er is een probleem met de installatie/connectiviteit van wachtwoordopschrijven
  - Er is een probleem met de installatie/connectiviteit van Azure AD-Verbinding maken
  - Zie Wachtwoordopschrijven oplossen voor meer stappen voor het oplossen van problemen met het terugschrijven van [wachtwoorden](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ik weet niet hoe ik het wachtwoord van een gebruiker opnieuw moet instellen**

1. Meld u aan bij de Azure-portal als een geschikte beheerder.
2. Ga naar het **blad Gebruikers en groepen** en selecteer Alle **gebruikers.**
3. Selecteer een gebruiker in de lijst.
4. Voor de geselecteerde gebruiker **selecteert** u Overzicht en selecteert u vervolgens in de opdrachtbalk **Wachtwoord opnieuw instellen.**
5. Selecteer de **knop Wachtwoord opnieuw** instellen en volg de instructies op het scherm.
    - Alleen resets die zijn uitgevoerd via de **wachtwoordschrijven** van azure portalondersteuning.

**Ik stel het wachtwoord van een on-premises gebruiker opnieuw in vanuit de Office 365 Admin portal of Office 365 mobiele toepassing, maar de gebruiker kan zich nog steeds niet aanmelden**

Password Writeback wordt niet ondersteund in deze portal. Stel het wachtwoord van de gebruiker opnieuw in in de Azure-portal.
