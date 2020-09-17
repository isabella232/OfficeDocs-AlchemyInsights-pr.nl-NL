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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777672"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan het primaire e-mailadres niet instellen, gebruikerskenmerken wijzigen of een gesynchroniseerde gebruiker verwijderen/verwijderen

Als adreslijstsynchronisatie is ingeschakeld voor uw omgeving, kunnen sommige kenmerken van gebruikers of objecten niet worden gewijzigd met het Microsoft 365-Beheercentrum.

Als u gesynchroniseerde gebruikers en alle bijbehorende kenmerken volledig wilt beheren, gebruikt u de lokale Active Directory-gebruikers en groepen beheerconsole (adsiedit. msc).  

U kunt ook individuele gebruikers of kenmerken wijzigen voor gesynchroniseerde gebruikers met behulp van PowerShell, zoals in deze algemene voorbeelden: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
