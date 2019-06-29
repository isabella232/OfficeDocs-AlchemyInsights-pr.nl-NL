---
title: Gesynchroniseerde gebruiker beheren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380500"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Niet primair e-mailadres instellen of wijzigen van gebruikerskenmerken

Als directory-synchronisatie is ingeschakeld voor uw omgeving kunnen niet bepaalde kenmerken van de gebruiker of het object worden gewijzigd met behulp van de Admin Center.
Volledig beheer van gesynchroniseerde gebruikers en alle bijbehorende kenmerken, uw lokale active directory-gebruikers en groepen management console gebruiken (adsiedit.msc).  

Ook kunt u afzonderlijke gebruikers of kenmerken voor gesynchroniseerde gebruikers met powershell, zoals weergegeven in de volgende veelvoorkomende voorbeelden: 
- Set MsolUser UserPrincipalName - user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com' - DisplayName "Het testgebruiker" - Achternaam 'Gebruiker'-titel "Manager"-afdeling "HR"
- Verwijderen MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com