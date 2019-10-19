---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545156"
---
# <a name="issues-with-mfa"></a>Problemen met MFA
Er zijn een aantal dingen om te controleren of gebruikers kunnen niet inloggen met multi-factor Authentication (MFA)

1. De betrokken gebruiker kan worden geblokkeerd in azure Active Directory-Portal. Als dat het geval is, wordt verificatiepogingen voor die specifieke gebruiker automatisch geweigerd. [Volg de stappen in dit artikel om deze te deblokkeren.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Als het deblokkeren van de gebruiker niet Help of de gebruiker niet is geblokkeerd, u proberen om MFA voor de gebruiker opnieuw in te stellen en zij zullen het proces voor inschrijven opnieuw doorlopen. [Volg de stappen in dit artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Als dit de eerste keer dat u MFA hebt ingeschakeld en uw gebruikers niet kunnen aanmelden bij niet-browsers clients zoals Outlook, Skype, enzovoort, is misschien ADAL (Active Directory Authentication Library) niet ingeschakeld op uw O365-abonnement. In dit geval moet u verbinding maken met Exchange Online PowerShell en deze cmdlet uitvoeren:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*