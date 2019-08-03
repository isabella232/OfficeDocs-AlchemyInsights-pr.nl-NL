---
title: Problemen met de MVR gesloten
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250160"
---
# <a name="issues-with-mfa"></a>Problemen met de MVR gesloten
Er zijn een paar dingen om te controleren als gebruikers kunnen zich niet aanmelden met behulp van meerledige verificatie (MVR gesloten)

1. De gebruiker kan worden geblokkeerd in Azure Active Directory-Portal. Als dit het geval is, probeert verificatie voor die specifieke gebruiker automatisch worden geweigerd. [Volg de stappen in dit artikel om de blokkering op te heffen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Als de gebruiker deblokkeren hebt gehad of niet door de gebruiker is geblokkeerd opnieuw instellen van de MVR gesloten voor de gebruiker kunt u proberen en ze weer inschrijven bij het opnieuw. [Volg de stappen in dit artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Als dit de eerste keer dat u ingeschakelde MVR gesloten en uw gebruikers zich niet aanmelden bij niet-browsers van clients zoals Outlook, Skype, enz, is misschien ADAL (Active Directory-verificatie Library) niet ingeschakeld op uw abonnement O365. In dit geval moet u verbinding maken met Exchange Online Powershell en voer deze cmdlet:  *Set OrganizationConfig-OAuth2ClientProfileEnabled: $true*