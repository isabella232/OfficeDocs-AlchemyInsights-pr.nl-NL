---
title: Wachtwoord schrijven werkt niet
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999739"
---
# <a name="password-writeback-is-not-working"></a>Wachtwoord schrijven werkt niet

**Ik heb problemen met het configureren van wachtwoordschrijven**

- Wachtwoord writeback is een premium-functie.
- Zorg ervoor dat u de licentievereisten begrijpt:
  - U moet ten minste één licentie hebben toegewezen in uw organisatie
  - **Alleen gebruikers in de** cloud: betaalde Office 365 (O365) of Azure AD Basic
  - **Cloud- en/of on-premises** gebruikers - Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
    - Zie Licentievereisten voor [selfservicewachtwoord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) opnieuw instellen voor Azure AD voor meer informatie over licentievereisten.
- U hebt ten minste één beheerdersaccount en één testgebruikersaccount met een van de juiste licenties.
- U moet Azure AD-Verbinding maken verbinding maken met de primaire domeincontroller Emulator om wachtwoord te kunnen terugschrijven. U kunt Azure AD-Verbinding maken configureren om een primaire domeincontroller  te gebruiken door met de rechtermuisknop op de eigenschappen van de Active Directory-synchronisatieconnector te klikken en vervolgens adreslijstpartities **configureren te selecteren.** Zoek van hier naar de sectie verbindingsinstellingen voor **domeincontrollers** en vink het selectievakje alleen **voorkeursdomeincontrollers aan.**
  > [!NOTE]
  > Als de voorkeurs-DC geen PDC-emulator is, neemt Azure AD Verbinding maken nog steeds contact op met de PDC voor het terugschrijven van wachtwoorden.
- Wachtwoord opnieuw instellen is geconfigureerd en ingeschakeld in uw tenant. Zie Gebruikers inschakelen [om hun Azure AD-wachtwoorden opnieuw in te stellen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)voor meer informatie.
- Zorg ervoor dat het beheerdersaccount dat wordt gebruikt voor het inschakelen van Password Writeback een cloudbeheerderaccount is (gemaakt in Azure AD en niet on-premises AD)
- U hebt één on-premises implementatie met meerdere of meerdere forest AD-implementaties Windows Server 2008 R2, Windows Server 2012 of Windows Server 2012 R2 met de nieuwste servicepakketten geïnstalleerd
- U hebt het hulpprogramma Azure AD Verbinding maken geïnstalleerd en u hebt uw AD-omgeving voorbereid voor synchronisatie met de cloud. Voordat u wachtwoord writeback test, moet u eerst een volledige import en volledige synchronisatie uitvoeren van zowel AD als Azure AD in Azure AD Verbinding maken.
- Zie voor meer informatie hoe u een volledige synchronisatie en volledige [import kunt uitvoeren in Azure AD Verbinding maken](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Ik heb een probleem met de connectiviteit voor het terugschrijven van wachtwoorden**

1. De nieuwste versie van [Azure AD-Verbinding maken](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallconfiguratie: Het hulpprogramma Azure AD Verbinding maken (1.1.443 en hoger) heeft **uitgaande HTTPS-toegang** nodig tot:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Toestaan dat inactieve verbindingen minimaal 2-3 minuten blijven bestaan

**Ik heb nog steeds problemen met het terugschrijven van wachtwoorden**

- Als u nog steeds problemen hebt, kunt u de wachtwoordschrijvenservice uitschakelen en opnieuw inschakelen in het hulpprogramma Azure AD Verbinding maken.
- Zie voor meer informatie hoe u wachtwoordschrijven kunt uitschakelen en [opnieuw inschakelen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
