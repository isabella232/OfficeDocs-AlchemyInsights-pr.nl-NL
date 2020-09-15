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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704484"
---
# <a name="configure-sync-features"></a>Synchronisatiefuncties configureren

Azure AD Connect bevat diverse functies die standaard zijn ingeschakeld, of die u later kunt inschakelen. Voor bepaalde functies is extra configuratie in specifieke omgevingen vereist.

- Limieten voor [filteren](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) de objecten worden gesynchroniseerd met Azure AD. Standaard worden alle gebruikers, contactpersonen, groepen en Windows 10-computeraccounts gesynchroniseerd. U kunt objecten opnemen of uitsluiten op basis van domeinen, Ou's of andere kenmerken.

- [Synchronisatie van wachtwoord hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoord-hash van de on-premises Active Directory naar Azure AD. Dit betekent dat het wachtwoord op één locatie kan worden gebruikt, maar het gebruik van hetzelfde wachtwoord in zowel on-premises als in Cloud omgevingen. Aangezien Active Directory de gezaghebbende bron is, kunt u uw eigen wachtwoordbeleid gebruiken.

- Met [selfservice voor wachtwoordherstel (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kunnen gebruikers hun eigen wachtwoorden opnieuw instellen in de Cloud, terwijl ze nog steeds uw on-premises wachtwoordbeleid toepassen.

- Met [apparaat voor herschrijfing](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunt u geregistreerde apparaten in azure AD terugschrijven naar de on-premises Active Directory, zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.

- [Onopzettelijke verwijdering voorkomen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige objecten worden verwijderd (meer dan 500 objecten per synchronisatie). U kunt deze instelling wijzigen om te voldoen aan de behoeften van uw organisatie.

- [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor expres installaties en helpt u ervoor te zorgen dat uw versie van Azure AD Connect altijd up-to-date is.
