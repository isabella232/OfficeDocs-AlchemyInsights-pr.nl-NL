---
title: SMTP-verificatie en probleemoplossing inschakelen
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077646"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-verificatie en probleemoplossing inschakelen

Als u SMTP-verificatie wilt inschakelen voor een postvak of als u een fout 'Client niet geverifieerd' of 'Verificatie mislukt' of 'SmtpClientAuthentication' krijgt met code 5.7.57 of 5.7.3 of 5.7.139 wanneer u e-mail probeert door te sturen door een apparaat of toepassing te verifiëren met Microsoft 365, voert u deze drie acties uit om het probleem op te lossen:

1. Schakel de [Azure-beveiligings defaults uit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) door Beveiligingsinstellingen inschakelen te wijzigen **in** **Nee.**

    a. Meld u aan bij de Azure-portal als beveiligingsbeheerder, beheerder van voorwaardelijke toegang of globale beheerder.<BR/>
    b. Blader naar Azure Active Directory > **Eigenschappen.**<BR/>
    c. Selecteer **Beveiligingsinstellingen beheren.**<BR/>
    d. Stel **Beveiligingsinstellingen inschakelen in** op **Nee.**<BR/>
    e. Kies **Opslaan**.

2. [Smtp-inzending van client inschakelen](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) in het gelicentieerde postvak.

    a. Ga in Microsoft 365-beheercentrum naar **Actieve gebruikers** en selecteer de gebruiker.<BR/>
    b. Ga naar het tabblad E-mail en selecteer onder **E-mail-apps** de optie **E-mail-apps beheren.**<BR/>
    d. Controleer of **Geverifieerde SMTP** is ingeschakeld (ingeschakeld).<BR/>
    e. Selecteer **Wijzigingen opslaan**.<BR/>

3. [Meervoudige verificatie (MFA) uitschakelen in](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) het gelicentieerde postvak.

    a. Ga naar de Microsoft 365-beheercentrum en selecteer gebruikers actieve gebruikers in het  >  **linkernavigatiemenu.**<BR/>
    b. Selecteer **Meervoudige verificatie**.<BR/>
    c. Selecteer de gebruiker en schakel **Multi-Factor auth uit.**<BR/>
