---
title: Problemen met SSPR oplossen
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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429717"
---
# <a name="troubleshoot-sspr"></a>Problemen met SSPR oplossen

**Ik heb problemen met het configureren van wachtwoord opnieuw instellen**

- Als u beheerder bent en wilt weten hoe u selfservice voor wachtwoord opnieuw instellen kunt inschakelen, bekijkt u [Zelfstudie SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)inschakelen om het opnieuw instellen van wachtwoorden voor uw organisatie te configureren. U kunt ook de [licentievereisten bekijken.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Er moet ten minste één licentie zijn toegewezen in uw organisatie.
    - **Alleen gebruikers in de cloud:** betaalde SKU's voor Office 365 (O365) of Azure AD Basic
    - **Cloud- en/of on-premises** gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
- Lees onze veelgestelde vragen voor meer vragen over het zelf opnieuw instellen [van wachtwoorden.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik krijg een foutbericht**

Lees dit artikel voor veelvoorkomende fouten en hun oplossingen: Problemen met zelf opnieuw instellen [van wachtwoorden oplossen](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik heb een probleem met mijn beleid voor het opnieuw instellen van wachtwoorden**

- Als uw beleid voor wachtwoord opnieuw instellen zich niet gedraagt zoals verwacht, of als u vragen hebt over beleidsregels voor het opnieuw instellen van wachtwoorden, lees dan dit artikel: Wachtwoordbeleid en -beperkingen [in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Beleidsregels voor wachtwoord opnieuw instellen zijn niet van toepassing op beheerders. Microsoft dwingt een sterk standaard twee gate wachtwoord opnieuw instellen voor elke Azure-beheerdersrol af. Zorg ervoor dat u test met een gebruiker die geen beheerder is. Zie het volgende artikel voor meer informatie over het beleid voor het opnieuw instellen van [beheerders.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ik wil niet dat mijn gebruikers extra beveiligingsgegevens registreren voor het opnieuw instellen van wachtwoorden**

U kunt gegevens (e-mail- en telefoonkenmerken) voor uw gebruikers vooraf in vullen met behulp van een API, PowerShell of Azure AD Connect. Voor meer informatie:

- [Wachtwoord opnieuw instellen implementeren zonder dat gebruikers zich moeten registreren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Welke gegevens worden gebruikt bij het opnieuw instellen van wachtwoorden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ik wil dat mijn gebruikers aanvullende beveiligingsgegevens registreren voor het opnieuw instellen van wachtwoorden**

1. Uw gebruikers hun beveiligingsgegevens laten registreren voor selfservice voor het opnieuw instellen van wachtwoorden door ze naar de [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Nadat gegevens zijn ingevuld voor de gebruiker (door de gebruiker [](https://passwordreset.microsoftonline.com/) of door de beheerder), moet u uw gebruiker aka.ms/sspr zodat uw gebruikers kunnen worden gemachtigd om hun eigen wachtwoorden opnieuw in te stellen.
1. Als gebruikers nog steeds problemen ondervinden, zijn ze waarschijnlijk **federatief of** met een **wachtwoord-hash gesynchroniseerde** gebruikers. Dit betekent dat er waarschijnlijk een probleem is met de service Wachtwoord terugschrijven.