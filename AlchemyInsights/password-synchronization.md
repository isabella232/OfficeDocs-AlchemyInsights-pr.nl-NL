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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960830"
---
# <a name="password-synchronization"></a>Wachtwoordsynchronisatie

**Wachtwoordhashsynchronisatie werkt helemaal niet**

Sommige veelvoorkomende problemen die klanten ondervinden wanneer wachtwoordhashsynchronisatie niet werkt, zijn:

- Het Active Directory-account dat door Azure AD Verbinding maken wordt gebruikt om te communiceren  met on-premises Active Directory, wordt niet verleend als **repliceren** van adreslijstwijzigingen en Adreslijstwijzigingen repliceren Alle machtigingen, die nodig zijn voor wachtwoordsynchronisatie, worden niet verleend. U moet dit oplossen door deze machtigingen toe te kennen aan het Active Directory-account.
- Wachtwoordhashsynchronisatie is uitgeschakeld nadat een beheerder de  methode Gebruiker Sign-In heeft gewijzigd van Wachtwoordsynchronisatie in een andere optie, zoals Federatie met  **AD FS** in de wizard Azure AD Verbinding maken. U kunt dit oplossen door de functie wachtwoordhashsynchronisatie opnieuw in te stellen in de wizard Azure AD Verbinding maken.
- Verbindingsprobleem met on-premises Active Directory. Sommige domeincontrollers zijn bijvoorbeeld niet toegankelijk voor Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD Verbinding maken of de vereiste poorten worden geblokkeerd door Firewall. U moet dit oplossen door ervoor te zorgen dat de verbinding tussen de Azure AD Verbinding maken-server en de on-premises Active Directory correct werkt.
- Azure AD Verbinding maken server die momenteel in de faseringsmodus staat, waardoor de server niet in staat is om de wachtwoordhashes te gebruiken. Als u het probleem wilt oplossen, volgt u de stappen die worden beschreven in de sectie Wachtwoordsynchronisatie met [Azure AD Verbinding maken-synchronisatie oplossen :](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Er worden geen wachtwoorden gesynchroniseerd.

**Wachtwoordhashsynchronisatie werkt niet voor sommige van mijn gebruikers**

1. Als u merkt dat wachtwoordhash niet wordt  gesynchroniseerd voor een gebruiker, gebruikt u de probleemoplossingstaak in de Azure AD-Verbinding maken om het probleem te onderzoeken en op te lossen. Voer de volgende taken uit:

    a. [De probleemoplossingstaak uitvoeren in de wizard](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [De cmdlet voor probleemoplossing gebruiken om het probleem met wachtwoordhashsynchronisatie voor een specifiek gebruik te onderzoeken](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Het on-premises Active Directory User-object is ingeschakeld voor **Gebruiker moet het wachtwoord wijzigen bij de volgende aanmeldingsoptie.** Wanneer deze optie is ingeschakeld, krijgt de gebruiker een tijdelijk wachtwoord toegewezen en wordt hem gevraagd het wachtwoord bij de volgende aanmelding te wijzigen. Azure AD Verbinding maken synchroniseert geen tijdelijke wachtwoorden met Azure AD.

Als u het bovenstaande probleem wilt oplossen, voert u een van de volgende taken uit:

- Vraag de gebruiker zich aan te melden bij een on-premises toepassing (bijvoorbeeld Windows bureaublad) en het wachtwoord te wijzigen. Het nieuwe wachtwoord wordt gesynchroniseerd met Azure AD.
- Laat een beheerder het wachtwoord van de gebruiker bijwerken zonder de optie in te stellen Gebruiker moet het wachtwoord wijzigen bij de volgende aanmelding **en** het nieuwe wachtwoord delen met de gebruiker.

3. Het on-premises Active Directory-gebruikersobject is **niet correct** geconfigureerd voor objectsynchronisatie of wachtwoordsynchronisatie. Als u dit probleem wilt oplossen, volgt u de stappen die worden beschreven in de synchronisatie van wachtwoordhash oplossen met [Azure AD Verbinding maken synchroniseren.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







