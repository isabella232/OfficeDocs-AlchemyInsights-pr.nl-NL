---
title: Wachtwoordsynchronisatie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481443"
---
# <a name="password-synchronization"></a>Wachtwoordsynchronisatie

**Wachtwoord-hashsynchronisatie werkt helemaal niet**

Sommige veelvoorkomende problemen die klanten ondervinden wanneer wachtwoord-hashsynchronisatie niet werkt, zijn:

- Aan het Active Directory-account dat door Azure AD Connect  wordt gebruikt  om te communiceren met on-premises Active Directory worden geen machtigingen verleend voor Repliceren directorywijzigingen en Repliceren Van alle( die zijn vereist voor wachtwoordsynchronisatie). U moet dit oplossen door deze machtigingen aan het Active Directory-account te verlenen.
- Wachtwoord-hashsynchronisatie wordt uitgeschakeld nadat een beheerder de  methode User Sign-In heeft gewijzigd van Wachtwoordsynchronisatie in een andere optie, zoals Federatie  met **AD FS** in de wizard Azure AD Connect. U kunt dit oplossen door de functie voor wachtwoordhashsynchronisatie opnieuw in te stellen in de wizard Azure AD Connect.
- Verbindingsprobleem met on-premises Active Directory. Sommige domeincontrollers zijn bijvoorbeeld niet toegankelijk voor [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect, of de vereiste poorten worden geblokkeerd door Firewall. U moet dit oplossen door ervoor te zorgen dat de verbinding tussen de Azure AD Connect-server en de on-premises Active Directory correct werkt.
- De Azure AD Connect-server wordt momenteel in de testmodus uitgevoerd, waardoor de server geen toegang heeft tot de wachtwoordhashes. Om het probleem op te lossen, volgt u de stappen in sectie Problemen met wachtwoordsynchronisatie oplossen met [Azure AD Connect-synchronisatie -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Er worden geen wachtwoorden gesynchroniseerd.

**Wachtwoord-hashsynchronisatie werkt niet voor sommige van mijn gebruikers**

1. Als het u is opgevallen dat wachtwoordhash  niet wordt gesynchroniseerd voor een gebruiker, gebruikt u de probleemoplossingstaak in Azure AD Connect om het probleem te onderzoeken en op te lossen. Voer de volgende taken uit:

    a. [De taak voor probleemoplossing in de wizard uitvoeren](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Gebruik de cmdlet probleemoplossing om het probleem met wachtwoordhashsynchronisatie voor een specifiek gebruik te onderzoeken](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Het on-premises Active Directory User-object is ingeschakeld voor Gebruiker moet **het wachtwoord wijzigen bij de volgende aanmeldingsoptie.** Wanneer deze optie is ingeschakeld, krijgt de gebruiker een tijdelijk wachtwoord toegewezen en wordt hem of haar gevraagd het wachtwoord te wijzigen bij de volgende aanmelding. Tijdelijke wachtwoorden worden niet gesynchroniseerd met Azure AD.

Voer een van de volgende taken uit om het bovenstaande probleem op te lossen:

- Vraag de gebruiker zich aan te melden bij de on-premises toepassing (bijvoorbeeld Windows-bureaublad) en het wachtwoord te wijzigen. Het nieuwe wachtwoord wordt gesynchroniseerd met Azure AD.
- Laat een beheerder het wachtwoord van de gebruiker bijwerken zonder de optie in teschakelen. Gebruiker moet het wachtwoord wijzigen bij de volgende aanmelding en het nieuwe wachtwoord delen met de gebruiker.

3. Het on-premises Active Directory User-object is niet **correct** geconfigureerd voor objectsynchronisatie of wachtwoordsynchronisatie. Om dit probleem op te lossen, volgt u de stappen die worden beschreven in [wachtwoord-hashsynchronisatie oplossen met Azure AD Connect-synchronisatie.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







