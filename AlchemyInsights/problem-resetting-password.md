---
title: Probleem met het opnieuw instellen van wachtwoord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039961"
---
# <a name="problems-resetting-password"></a>Problemen met het opnieuw instellen van wachtwoord

Hieronder volgen enkele van de problemen waarmee u mogelijk te maken kunt krijgen bij het opnieuw instellen van het wachtwoord en de mogelijke oplossingen:

**Ik heb een probleem met het opnieuw instellen van wachtwoorden die niet worden behandeld in de andere categorieën**

- Controleer of u gemachtigd bent wachtwoorden opnieuw in te stellen. Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.
- Zorg ervoor dat u de licentievereisten begrijpt:
    - U moet ten minste één licentie hebben toegewezen in uw organisatie
        - Alleen gebruikers in de cloud: Office 365 (O365) betaalde SKU of Azure AD Basic
        - Cloud- en/of on-premises gebruikers - Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
        - Zie het artikel Licentievereisten voor selfservice voor Azure AD voor het opnieuw instellen van wachtwoorden voor Azure AD voor meer [informatie over licentievereisten.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik heb problemen met het testen van het beleid voor het opnieuw instellen van wachtwoorden dat ik heb ingesteld**

- Het kan enkele minuten duren voordat onlangs toegepaste beleidsregels in alle datacenters en eindpunten zijn gerepliceerd. Fysieke afstand tot het datacenter is ook van invloed op de manier waarop wijzigingen snel worden toegepast.
- Test met een eindgebruiker, niet met een beheerder, en test met een kleine set gebruikers. Het beleid dat is geconfigureerd in de Azure-portal, is alleen van toepassing op eindgebruikers, niet op beheerders. Microsoft dwingt een sterk standaard tweepoortsbeleid voor het opnieuw instellen van wachtwoorden af voor een Azure-beheerdersrol (bijvoorbeeld: globale beheerder, helpdeskbeheerder, wachtwoordbeheerder, enzovoort)
    - Meer informatie over [beleidsregels voor beheerders](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Ik wil wachtwoord opnieuw instellen, maar ik wil niet dat mijn gebruikers extra beveiligingsgegevens registreren**

Vul vooraf gegevens in voor uw gebruikers, zodat ze dat niet hoeven te doen. - Als beheerder kunt u telefoon- en e-maileigenschappen instellen voor uw gebruikers voordat u een wachtwoord opnieuw in uw organisatie uitrolt. U kunt dit doen met een API, PowerShell of Azure AD-Verbinding maken. Meer informatie vindt u hier:
- [Wachtwoord opnieuw instellen zonder dat gebruikers zich moeten registreren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Welke gegevens worden gebruikt bij het opnieuw instellen van wachtwoorden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**De knop Wachtwoord opnieuw instellen is grijs**

U bent niet gemachtigd om de wachtwoorden van deze gebruiker opnieuw in te stellen. Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.

**Ik zie het wachtwoord voor het opnieuw instellen van het mes niet**

U bent niet gemachtigd wachtwoorden opnieuw in te stellen. Alleen globale gebruikerswachtwoorden, wachtwoordbeheerders en gebruikersbeheerders kunnen gebruikerswachtwoorden opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoorrechte beheerders opnieuw instellen.

**Ik zie het on-premises integratieblad niet in het opnieuw instellen van wachtwoorden**

- Het on-premises integratieblad wordt alleen weergegeven in hybride omgevingen, wat betekent dat u wachtwoord writeback gebruikt om de wachtwoorden van on-premises gebruikers te manipuleren.
- U ziet dit blad niet als:
    - U gebruikt geen wachtwoord writeback
    - Er is een probleem met de installatie/connectiviteit van wachtwoordopschrijven
    - Er is een probleem met de installatie/connectiviteit van Azure AD-Verbinding maken
    - Zie de sectie Wachtwoordopschrijven oplossen voor meer stappen voor het oplossen van problemen met het [terugschrijven van wachtwoorden.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik weet niet hoe ik het wachtwoord van een gebruiker opnieuw moet instellen**

1. Meld u aan bij de Azure-portal als een geschikte beheerder.
1. Ga naar het blad Gebruikers en groepen en selecteer **Alle gebruikers.**
1. Selecteer een gebruiker in de lijst.
1. Voor de geselecteerde gebruiker **selecteert** u Overzicht en klikt u op de opdrachtbalk op **Wachtwoord opnieuw instellen.**
1. Volg de instructies op het scherm.
    - Alleen resets die zijn uitgevoerd via de wachtwoordschrijven van azure portalondersteuning.

**Ik stel het wachtwoord van een on-premises gebruiker opnieuw in vanuit de Office 365 Admin portal of Office 365 mobiele toepassing, maar de gebruiker kan zich nog steeds niet aanmelden**

Password Writeback wordt niet ondersteund in deze portal. Het wachtwoord van de gebruiker opnieuw instellen in de Azure-portal - portal.azure.com

