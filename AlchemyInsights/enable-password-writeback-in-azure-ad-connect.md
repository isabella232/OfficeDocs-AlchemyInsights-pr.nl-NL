---
title: Wachtwoord terugschrijven inschakelen in Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814007"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Wachtwoord terugschrijven inschakelen in Azure AD Connect

Als u het zelf terugschrijven voor wachtwoordherstel wilt inschakelen, moet u eerst de optie terugschrijven inschakelen in Azure AD Connect. Voer de volgende stappen uit vanaf de Azure AD Connect-server:

1. Meld u aan bij de Azure AD Connect-server en start de **Azure AD Connect**-configuratiewizard.
2. Klik op de **welkomstpagina** op **Configureren**.
3. Klik op de pagina **Aanvullende taken** op **Synchronisatieopties aanpassen** en klik dan op **Volgende**.
4. Voer op de pagina **Verbinding maken met Azure AD** de referenties van de globale beheerder voor uw Azure-tenant in en klik vervolgens op **Volgende**.
5. Klik op de pagina's **Mappen verbinden** en **Domein/OE filteren** op **Volgende**.
6. Selecteer op de pagina **Optionele functies** het vakje naast **Wachtwoord terugschrijven** en klik op **Volgende**.
7. Klik op de pagina **Klaar om te configureren** op **Configureren** en wacht tot het proces is voltooid.
8. Wanneer u ziet dat de configuratie is voltooid, klikt u op **Afsluiten**.

Wanneer het terugschrijven van wachtwoorden is ingeschakeld in Azure AD Connect, configureert u Azure AD SSPR voor terugschrijven.  Voer de volgende stappen uit om het terugschrijven van wachtwoorden in SSPR in te schakelen:

1. Meld u aan bij Azure Portal met het globale beheerdersaccount.
2. Zoek en selecteer **Azure Active Directory**, klik op **Wachtwoord opnieuw instellen** en klik vervolgens op **On-premises integratie**.
3. Stel de optie voor **Wachtwoorden terugschrijven naar uw on-premises directory?** in op **Ja**.
4. Stel de optie voor **Gebruikers toestaan accounts te ontgrendelen zonder het wachtwoord opnieuw in te stellen?** in op **Ja**.
5. Wanneer u klaar bent, klikt u op **Opslaan**.

Zie [Zelf in Azure Active Directory terugschrijven voor wachtwoordherstel naar een on-premises omgeving inschakelen](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback) voor meer informatie.

> [!NOTE]
>  Wanneer een beheerder het wachtwoord van een gebruiker opnieuw instelt in Azure Portal, wordt het wachtwoord teruggeschreven naar on-premises bij een federatieve gebruiker of synchronisatie met een wachtwoord-hash. Deze functionaliteit vereist een Azure Premium-licentie (P1 of P2) en wordt momenteel niet ondersteund op de Office-beheerportal.
