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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768832"
---
# <a name="issues-with-azure-mfa"></a>Problemen met Azure MFA
Er zijn een aantal dingen om te controleren of gebruikers kunnen niet aanmelden met multi-factor Authentication (MFA)

1. De betrokken gebruiker kan worden geblokkeerd in azure Active Directory-Portal. Als dat het geval is, wordt verificatiepogingen voor die specifieke gebruiker automatisch geweigerd. [Volg de stappen in dit artikel om deze te deblokkeren.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Als het deblokkeren van de gebruiker niet Help of de gebruiker niet is geblokkeerd, u proberen om MFA voor de gebruiker opnieuw in te stellen en zij zullen het proces voor inschrijven opnieuw doorlopen. [Volg de stappen in dit artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Als dit de eerste keer dat u MFA hebt ingeschakeld en uw gebruikers niet kunnen aanmelden bij niet-browsers clients zoals Outlook, Skype, enzovoort, is misschien ADAL (Active Directory Authentication Library) niet ingeschakeld op uw O365-abonnement. In dit geval moet u verbinding maken met Exchange Online PowerShell en deze cmdlet uitvoeren:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*