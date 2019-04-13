---
title: 646 het configureren van AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856651"
---
# <a name="configure-sync-features"></a>Synchronisatiefuncties configureren

Azure AD Connect bevat diverse functies die standaard zijn ingeschakeld, of dat u later kunt inschakelen. Sommige functies vereisen aanvullende configuratie specifieke omgevingen.

- [Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limieten voor de objecten worden gesynchroniseerd met Azure AD. Standaard alle gebruikers, contactpersonen, groepen en Windows 10 worden computeraccounts gesynchroniseerd. U kunt opnemen of uitsluiten objecten op basis van domeinen, organisatie-eenheden of andere kenmerken.

- [Wachtwoord hash-synchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoordhash naar Azure AD van Active Directory op gebouwen. Daardoor kan het wachtwoord management op één locatie, maar gebruik van het wachtwoord in beide op gebouwen en cloud-omgevingen. Omdat Active Directory de bindende bron is, kunt u uw eigen instellingen voor wachtwoordbeleid.

- [Self-wachtwoord opnieuw instellen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kunnen gebruikers hun wachtwoorden in de cloud tijdens het toepassen van het wachtwoordbeleid op de gebouwen nog steeds opnieuw.

- [Apparaat writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunnen geregistreerde apparaten in Azure AD terug naar Active Directory op de ruimten worden geschreven zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.

- [Voorkomen dat per ongeluk wordt verwijderd](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige object verwijderen (meer dan 500 objecten per synchronisatie). U kunt deze instelling om te voldoen aan de behoeften van uw organisatie.

- [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor snelle installatie en zorgt ervoor dat uw versie van Azure AD verbinden altijd actueel is.
