---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755126"
---
# <a name="issues-with-azure-mfa"></a>Problemen met Azure MFA
Er zijn enkele dingen die u kunt controleren als gebruikers zich niet kunnen aanmelden met multi-factor Authentication (MFA)

1. De betrokken gebruiker wordt mogelijk geblokkeerd in azure Active Directory Portal. Als dat het geval is, worden verificatiepogingen voor die specifieke gebruiker automatisch geweigerd. [Voer de stappen in dit artikel uit om ze te deblokkeren.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Als het deblokkeren van de gebruiker niet is gelukt of als de gebruiker niet is geblokkeerd, kunt u proberen MFA opnieuw in te stellen voor de gebruiker, zodat ze opnieuw de registratieprocedure doorlopen. [Voer de stappen in dit artikel uit.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Als dit de eerste keer is dat u MFA inschakelt en uw gebruikers niet kunnen inloggen met niet-browsers, zoals Outlook, Skype, etc, of ADAL (Active Directory Authentication Library), is niet ingeschakeld voor uw O365-abonnement. In dit geval dient u verbinding te maken met Exchange Online PowerShell en deze cmdlet uit te voeren:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*