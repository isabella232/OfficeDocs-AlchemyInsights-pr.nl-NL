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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541981"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Niet primair e-mailadres instellen of wijzigen van gebruikerskenmerken

Als directory-synchronisatie is ingeschakeld voor uw omgeving, kunnen niet enkele kenmerken van de gebruiker of het object worden gewijzigd met behulp van het Microsoft 365 admin center.

Volledig beheer van gesynchroniseerde gebruikers en alle bijbehorende kenmerken, uw lokale active directory-gebruikers en groepen management console gebruiken (adsiedit.msc).  

Ook kunt u afzonderlijke gebruikers of kenmerken voor gesynchroniseerde gebruikers met powershell, zoals weergegeven in de volgende veelvoorkomende voorbeelden: 
- Set MsolUser UserPrincipalName - user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com' - DisplayName "Het testgebruiker" - Achternaam 'Gebruiker'-titel "Manager"-afdeling "HR"
- Verwijderen MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com