---
title: Gesynchroniseerde gebruiker beheren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451395"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan het primaire e-mailadres niet instellen, gebruikerskenmerken wijzigen of een gesynchroniseerde gebruiker verwijderen/verwijderen

Als adreslijstsynchronisatie is ingeschakeld voor uw omgeving, kunnen sommige kenmerken van gebruikers of objecten niet worden gewijzigd met het Microsoft 365-Beheercentrum.

Als u gesynchroniseerde gebruikers en alle bijbehorende kenmerken volledig wilt beheren, gebruikt u de lokale Active Directory-gebruikers en groepen beheerconsole (adsiedit. msc).  

U kunt ook individuele gebruikers of kenmerken wijzigen voor gesynchroniseerde gebruikers met behulp van PowerShell, zoals in deze algemene voorbeelden:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
