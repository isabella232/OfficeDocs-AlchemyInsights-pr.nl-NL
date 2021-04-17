---
title: Gesynchroniseerde gebruiker beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823962"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan geen primair e-mailadres instellen, gebruikerskenmerken wijzigen of een gesynchroniseerde gebruiker verwijderen/verwijderen

Als adreslijstsynchronisatie is ingeschakeld voor uw omgeving, kunnen bepaalde gebruikers- of objectkenmerken niet worden gewijzigd via het Microsoft 365-beheercentrum.

Als u gesynchroniseerde gebruikers en al hun kenmerken volledig wilt beheren, gebruikt u uw lokale active directory-gebruikers en groepenbeheerconsole (adsiedit.msc).  

U kunt ook afzonderlijke gebruikers of kenmerken voor gesynchroniseerde gebruikers wijzigen met powershell, zoals wordt weergegeven in deze veelvoorkomende voorbeelden:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
