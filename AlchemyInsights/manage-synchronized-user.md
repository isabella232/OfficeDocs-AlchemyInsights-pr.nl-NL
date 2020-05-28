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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407345"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan geen primair e-mailadres instellen, gebruikerskenmerken wijzigen of een gesynchroniseerde gebruiker verwijderen/verwijderen

Als adreslijstsynchronisatie is ingeschakeld voor uw omgeving, kunnen sommige gebruikers- of objectkenmerken niet worden gewijzigd met het Microsoft 365-beheercentrum.

Als u gesynchroniseerde gebruikers en al hun kenmerken volledig wilt beheren, gebruikt u uw lokale active directory-gebruikers- en groepsbeheerconsole (adsiedit.msc).  

U ook afzonderlijke gebruikers of kenmerken voor gesynchroniseerde gebruikers wijzigen met behulp van powershell, zoals weergegeven in deze algemene voorbeelden: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
