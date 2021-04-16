---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810479"
---
# <a name="issues-with-azure-mfa"></a>Problemen met Azure MFA
Er zijn een paar dingen om te controleren of gebruikers zich niet kunnen aanmelden met meervoudige verificatie (MFA)

1. De betreffende gebruiker kan worden geblokkeerd in Azure Active Directory Portal. Als dat het geval is, worden verificatiepogingen voor die specifieke gebruiker automatisch geweigerd. [Volg de stappen in dit artikel om de blokkering te deblokkeren.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Als het deblokkeren van de gebruiker niet heeft geholpen of de gebruiker niet is geblokkeerd, kunt u proberen MFA opnieuw in te stellen voor de gebruiker en wordt het registratieproces opnieuw doorlopen. [Volg de stappen in dit artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Als dit de eerste keer is dat u MFA inschakelen en uw gebruikers zich niet kunnen aanmelden bij niet-browsers,zoals Outlook, Skype, enzovoort, is ADAL (Active Directory Authentication Library) mogelijk niet ingeschakeld op uw O365-abonnement. In dit geval moet u verbinding maken met Exchange Online Powershell en deze cmdlet uitvoeren:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*