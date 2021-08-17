---
title: SSPR oplossen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038953"
---
# <a name="troubleshoot-sspr"></a>SSPR oplossen

**Ik heb problemen met het configureren van het opnieuw instellen van wachtwoorden**

- Als u beheerder bent en wilt weten hoe u het opnieuw instellen van selfservicewachtwoord kunt inschakelen, zie [Zelfstudie SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)inschakelen , om wachtwoord opnieuw instellen voor uw organisatie te configureren. Mogelijk wilt u ook de [licentievereisten bekijken.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Er moet ten minste één licentie zijn toegewezen in uw organisatie.
    - **Alleen gebruikers in de** cloud: betaalde Office 365 (O365) of Azure AD Basic
    - **Cloud- en/of on-premises** gebruikers - Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
- Lees onze veelgestelde vragen voor meer vragen over het opnieuw instellen van [selfservicewachtwoord.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik krijg een foutbericht**

Lees dit artikel om veelvoorkomende fouten en hun oplossingen te vinden: [Problemen met het opnieuw instellen van selfservicewachtwoord oplossen](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik heb een probleem met mijn beleid voor het opnieuw instellen van wachtwoorden**

- Als uw beleid voor het opnieuw instellen van wachtwoorden niet werkt zoals verwacht, of als u vragen hebt over beleid voor het opnieuw instellen van wachtwoorden, bekijkt u dit artikel: Wachtwoordbeleid en [-beperkingen in](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)Azure Active Directory.
- Beleid voor het opnieuw instellen van wachtwoorden is niet van toepassing op beheerders. Microsoft dwingt een sterk standaard tweepoortsbeleid voor het opnieuw instellen van wachtwoorden af voor elke Azure-beheerdersrol. Zorg ervoor dat u test met een gebruiker die geen beheerder is. Zie dit artikel: Beleidsverschillen opnieuw instellen voor beheerders voor meer informatie over het beleid voor het opnieuw instellen van [beheerders.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ik wil niet dat mijn gebruikers extra beveiligingsgegevens registreren voor het opnieuw instellen van wachtwoorden**

U kunt gegevens (e-mail- en telefoonkenmerken) vooraf in vullen voor uw gebruikers met behulp van een API, PowerShell of Azure AD-Verbinding maken. Lees het volgende voor meer informatie:

- [Wachtwoord opnieuw instellen zonder dat gebruikers zich moeten registreren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Welke gegevens worden gebruikt bij het opnieuw instellen van wachtwoorden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik wil dat mijn gebruikers hun extra beveiligingsgegevens registreren voor het opnieuw instellen van wachtwoorden**

1. Uw gebruikers hun beveiligingsgegevens laten registreren voor het opnieuw instellen van selfservicewachtwoord door ze te sturen naar [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Nadat gegevens zijn ingevuld voor de gebruiker (door de gebruiker of door de beheerder), stuurt u uw gebruiker naar [aka.ms/sspr](https://passwordreset.microsoftonline.com/) zodat uw gebruikers de bevoegdheid hebben hun eigen wachtwoorden opnieuw in te stellen.
1. Als gebruikers nog steeds problemen ondervinden, zijn ze waarschijnlijk **federatief** of **wachtwoordhashsynchrone** gebruikers. Dit betekent dat er waarschijnlijk een probleem is met de service Password Writeback.