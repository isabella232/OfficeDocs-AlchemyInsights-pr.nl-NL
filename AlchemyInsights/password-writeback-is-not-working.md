---
title: Wachtwoord terugschrijven werkt niet
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243289"
---
# <a name="password-writeback-is-not-working"></a>Wachtwoord terugschrijven werkt niet

**Ik heb problemen met het configureren van wachtwoordin writeback**

- Wachtwoord terugschrijven is een premium-functie.
- Zorg ervoor dat u de licentievereisten begrijpt:
  - Er moet ten minste één licentie zijn toegewezen in uw organisatie
  - **Alleen cloudgebruikers:** betaalde SKU's voor Office 365 (O365) of Azure AD Basic
  - **Cloud- en/of on-premises** gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)
    - Zie Licentievereisten voor selfservice voor wachtwoord opnieuw instellen voor Azure AD voor meer informatie [over licentievereisten](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- U hebt ten minste één beheerdersaccount en één gebruikersaccount voor de test met een van de juiste licenties.
- U moet Azure AD Connect verbinden met de Primaire domeincontroller Emulator om terugschrijven van wachtwoorden te laten werken. U kunt Azure AD Connect configureren voor het gebruik  van een primaire domeincontroller door met de rechtermuisknop op de eigenschappen van de Active Directory-synchronisatieconnector te klikken en vervolgens adreslijstpartities **configureren te selecteren.** Zoek hier de sectie verbindingsinstellingen voor de **domeincontroller** en vink het selectievakje aan met de naam **Alleen voorkeursdomeincontrollers gebruiken.**
  > [!NOTE]
  > Als de voorkeurs-DC geen PDC-emulator is, neemt Azure AD Connect nog steeds contact op met de PDC voor terugschrijven met een wachtwoord.
- Wachtwoord opnieuw instellen is geconfigureerd en ingeschakeld in uw tenant. Zie Gebruikers in staat stellen [hun Azure AD-wachtwoorden opnieuw in te stellen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)voor meer informatie.
- Zorg ervoor dat het administratoraccount dat wordt gebruikt voor het inschakelen van Wachtwoord terugschrijven een cloudbeheerdersaccount is (gemaakt in Azure AD, niet on-premises AD)
- U hebt één on-premises implementatie of een on-premises AD-implementatie voor meerdere forest uitgevoerd Windows Server 2008 R2, Windows Server 2012 of Windows Server 2012 R2 met de nieuwste servicepacks geïnstalleerd
- U hebt het hulpprogramma Azure AD Connect geïnstalleerd en u hebt uw AD-omgeving voorbereid voor synchronisatie met de cloud. Voordat u wachtwoordschrijven test, moet u eerst een volledige import en volledige synchronisatie uitvoeren vanuit AD en Azure AD in Azure AD Connect.
- Voor meer informatie, zie hoe u een volledige synchronisatie en volledige [import in Azure AD Connect kunt uitvoeren](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Ik heb een probleem met de connectiviteit voor terugschrijven met wachtwoorden**

1. De nieuwste versie van [Azure AD Connect downloaden en inschakelen](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallconfiguratie: Het hulpprogramma Azure AD Connect (1.1.443 en hoger) heeft uitgaande **HTTPS-toegang** nodig voor:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Inactieve verbindingen ten minste 2-3 minuten laten aanhouden

**Ik heb nog steeds problemen met het terugschrijven van wachtwoorden**

- Als u nog steeds problemen hebt, kunt u proberen de service voor wachtwoordschrijven in het hulpprogramma Azure AD Connect uit te stellen en opnieuw in teschakelen.
- Voor meer informatie, zie hoe u wachtwoordschrijven uit- en [opnieuw inschakelen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
