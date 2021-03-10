---
title: Probleem bij het opnieuw instellen van wachtwoord
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693391"
---
# <a name="problems-resetting-password"></a>Problemen bij het opnieuw instellen van het wachtwoord

Hier volgen enkele problemen die kunnen voorkomen bij het opnieuw instellen van het wachtwoord en de mogelijke oplossingen:

**Ik heb een probleem met wachtwoord opnieuw instellen, dat niet wordt gedekt in de andere categorieën**

- Controleer of u bent gemachtigd om wachtwoorden opnieuw in te stellen. Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.
- Zorg ervoor dat u de licentievereisten begrijpt:
    - Er moet ten minste één licentie zijn toegewezen in uw organisatie
        - Alleen cloudgebruikers: betaalde SKU's voor Office 365 (O365) of Azure AD Basic
        - Cloud- en/of on-premises gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
        - Zie het artikel Licentievereisten voor selfservice voor het opnieuw instellen van wachtwoorden voor Azure AD voor meer informatie over [licentievereisten.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik heb problemen met het testen van het beleid voor het opnieuw instellen van wachtwoorden dat ik heb ingesteld**

- Het kan enkele minuten duren voordat onlangs toegepaste beleidsregels zijn gerepliceerd in alle datacenters en eindpunten. Fysieke afstand tot het datacenter is ook van invloed op hoe snel wijzigingen worden toegepast.
- Test met een eindgebruiker, niet een beheerder, en test met een kleine groep gebruikers. De beleidsregels die in de Azure Portal zijn geconfigureerd, zijn ALLEEN van toepassing op eindgebruikers, niet op beheerders. Microsoft dwingt een sterk standaard twee gate wachtwoord opnieuw instellen af voor elke Azure-beheerdersrol (bijvoorbeeld: globale beheerder, helpdeskbeheerder, wachtwoordbeheerder, enzovoort).
    - Meer informatie over [beleid voor beheerders.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Ik wil het opnieuw instellen van wachtwoorden implementeren, maar ik wil niet dat mijn gebruikers aanvullende beveiligingsgegevens registreren**

Vul vooraf gegevens in voor uw gebruikers, zodat u dat zelf niet hoeft te doen. - Als beheerder kunt u telefoon- en e-maileigenschappen instellen voor uw gebruikers voordat u het wachtwoord opnieuw in de organisatie uitrolt. U kunt dit doen met behulp van een API, PowerShell of Azure AD Connect. Meer informatie vindt u hier:
- [Wachtwoord opnieuw instellen implementeren zonder dat gebruikers zich moeten registreren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Welke gegevens worden gebruikt bij het opnieuw instellen van wachtwoorden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**De knop Wachtwoord opnieuw instellen heeft een grijze kleur**

U bent niet gemachtigd om wachtwoorden van deze gebruiker opnieuw in te stellen. Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.

**Ik zie het wachtwoord niet om het blade opnieuw in te stellen**

U bent niet gemachtigd om wachtwoorden opnieuw in te stellen. Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen. Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.

**Ik zie het on-premises integratie blade niet in wachtwoord opnieuw instellen**

- De on-premises integratie blade wordt alleen weergegeven in hybride omgevingen, wat betekent dat u wachtwoordschrijven gebruikt om on-premises gebruikerswachtwoorden te manipuleren.
- U ziet dit blade niet als:
    - U gebruikt wachtwoordschrijven niet
    - Er is een probleem met de installatie/connectiviteit van wachtwoordopschrijven
    - Er is een probleem met de installatie/connectiviteit van Azure AD Connect
    - Zie de sectie Problemen met wachtwoordopschrijven oplossen voor meer stappen voor het oplossen van problemen met [wachtwoordopschrijven](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik weet niet hoe ik het wachtwoord van een gebruiker opnieuw moet instellen**

1. Meld u aan bij de Azure Portal als een geschikte beheerder.
1. Ga naar de blade Gebruikers en groepen, selecteer **Alle gebruikers.**
1. Selecteer een gebruiker in de lijst.
1. Voor de geselecteerde gebruiker selecteert u **Overzicht** en klikt u op de opdrachtbalk op **Wachtwoord opnieuw instellen.**
1. Volg de instructies op het scherm.
    - Alleen resets die zijn uitgevoerd via de ondersteuning van Azure Portal bieden ondersteuning voor terugschrijven van wachtwoorden.

**Ik stel het wachtwoord van een on-premises gebruiker opnieuw in vanuit de Office 365-beheerportal of de mobiele Office 365-toepassing, maar de gebruiker kan zich nog steeds niet aanmelden**

Wachtwoord terugschrijven wordt niet ondersteund in deze portal. Het wachtwoord van de gebruiker opnieuw instellen in azure portal - portal.azure.com

