---
title: 646 AADConnect configureren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963638"
---
# <a name="configure-sync-features"></a>Synchronisatiefuncties configureren

Azure AD Verbinding maken bevat verschillende functies die standaard zijn ingeschakeld of die u later kunt inschakelen. Sommige functies vereisen extra configuratie in specifieke omgevingen.

- [Filterlimieten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) de objecten worden gesynchroniseerd met Azure AD. Standaard worden alle gebruikers, contactpersonen, groepen en Windows 10 computeraccounts gesynchroniseerd. U kunt objecten opnemen of uitsluiten op basis van domeinen, OUs's of andere kenmerken.

- [Wachtwoordhashsynchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoordhash van de on-premises Active Directory naar Azure AD. Hierdoor kan wachtwoordbeheer op één locatie worden gebruikt, maar wordt hetzelfde wachtwoord gebruikt in zowel on-premises omgevingen als cloudomgevingen. Omdat Active Directory de gezaghebbende bron is, kunt u uw eigen wachtwoordbeleid gebruiken.

- [Met SelfService Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kunnen gebruikers hun eigen wachtwoorden opnieuw instellen in de cloud terwijl ze nog steeds uw on-premises wachtwoordbeleid toepassen.

- [Met apparaatschrijven](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunnen geregistreerde apparaten in Azure AD worden teruggeschreven naar de on-premises Active Directory, zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.

- [Voorkomen dat u per](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ongeluk verwijdert, is standaard ingeschakeld om te voorkomen dat er te veel objecten tegelijk worden verwijderd (meer dan 500 objecten per synchronisatie). U kunt deze instelling wijzigen om aan de behoeften van uw organisatie te voldoen.

- [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor express-installaties en helpt ervoor te zorgen dat uw versie van Azure AD-Verbinding maken altijd actueel is.
