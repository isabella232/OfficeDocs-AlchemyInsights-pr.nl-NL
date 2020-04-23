---
title: 646 AadConnect configureren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722528"
---
# <a name="configure-sync-features"></a>Synchronisatiefuncties configureren

Azure AD Connect bevat verschillende functies die standaard zijn ingeschakeld of die u later inschakelen. Sommige functies vereisen extra configuratie in specifieke omgevingen.

- [Filterlimieten de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objecten worden gesynchroniseerd met Azure AD. Standaard worden alle gebruikers, contactpersonen, groepen en Windows 10-computeraccounts gesynchroniseerd. U objecten opnemen of uitsluiten op basis van domeinen, OU's of andere kenmerken.

- [Synchronisatie van wachtwoordhash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoordhash van de on-premises Active Directory naar Azure AD. Dit maakt wachtwoordbeheer op één locatie mogelijk, maar het gebruik van hetzelfde wachtwoord in zowel on-premises als cloudomgevingen. Omdat Active Directory de gezaghebbende bron is, u uw eigen wachtwoordbeleid gebruiken.

- [Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) stelt gebruikers in staat om hun eigen wachtwoorden opnieuw in de cloud te resetten terwijl ze nog steeds uw on-premises wachtwoordbeleid toepassen.

- [Met apparaatterugschrijftijd](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunnen geregistreerde apparaten in Azure AD worden teruggeschreven naar de on-premises Active Directory, zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.

- [Voorkomen dat per ongeluk worden](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) verwijderd, is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige objectverwijderingen (meer dan 500 objecten per synchronisatie) worden verwijderd. U deze instelling wijzigen om aan de behoeften van uw organisatie te voldoen.

- [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor expresinstallaties en zorgt ervoor dat uw versie van Azure AD Connect altijd actueel is.
