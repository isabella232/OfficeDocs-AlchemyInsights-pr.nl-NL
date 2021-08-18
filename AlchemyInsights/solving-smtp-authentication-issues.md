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
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321748"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-verificatie en probleemoplossing inschakelen

Als u SMTP-verificatie wilt inschakelen voor een postvak of als u een fout 'Client niet geverifieerd' of 'Verificatie mislukt' of 'SmtpClientAuthentication' krijgt met code 5.7.57 of 5.7.3 of 5.7.139 wanneer u e-mail probeert door te sturen door een apparaat of toepassing te verifiëren met Microsoft 365, voert u deze drie acties uit om het probleem op te lossen:

1. Schakel de [Azure-beveiligings defaults uit](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) door Beveiligingsinstellingen inschakelen te wijzigen **in** **Nee.**

    a. Meld u aan bij de Azure-portal als beveiligingsbeheerder, beheerder van voorwaardelijke toegang of globale beheerder.<BR/>
    b. Blader naar Azure Active Directory > **eigenschappen.**<BR/>
    c. Selecteer **Beveiligingsinstellingen beheren.**<BR/>
    d. Stel **Beveiligingsinstellingen inschakelen in** op **Nee.**<BR/>
    e. Selecteer **Opslaan**.

2. [Smtp-clientinzending inschakelen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) voor het gelicentieerde postvak.

    a. Ga in Microsoft 365-beheercentrum naar **Actieve gebruikers** en selecteer de gebruiker.<BR/>
    b. Ga naar het tabblad E-mail en selecteer onder **E-mail-apps** de optie **E-mail-apps beheren.**<BR/>
    d. Controleer of **Geverifieerde SMTP** is ingeschakeld (ingeschakeld).<BR/>
    e. Selecteer **Wijzigingen opslaan**.<BR/>

3. [Meervoudige verificatie (MFA) uitschakelen in](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) het gelicentieerde postvak.

    a. Ga naar het Microsoft 365-beheercentrum en selecteer gebruikers actieve gebruikers in het  >  **linkernavigatiemenu.**<BR/>
    b. Selecteer **Meervoudige verificatie**.<BR/>
    c. Selecteer de gebruiker en schakel **Multi-Factor auth uit.**<BR/>
