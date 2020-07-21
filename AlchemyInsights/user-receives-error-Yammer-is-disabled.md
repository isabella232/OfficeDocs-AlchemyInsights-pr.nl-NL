---
title: Gebruiker ontvangt fout AADSTS7000112 Yammer is uitgeschakeld
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197873"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Gebruiker ontvangt fout AADSTS7000112 Yammer is uitgeschakeld

Als u de foutmelding "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000000'(Yammer) ontvangt, is er een probleem met de servicehoofdpaal binnen Azure AD. Een beheerder heeft mogelijk de servicehoofdsom uitgeschakeld om de toegang tot Yammer te blokkeren.

Het uitschakelen van de service principal wordt niet aanbevolen en kan extra problemen veroorzaken. Zie [Yammer-toegang uitschakelen voor Microsoft 365-gebruikers voor](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)meer informatie over de ondersteunde aanpak om de toegang van gebruikers tot Yammer te blokkeren.  

Ga als volgt te werk om dit probleem in de Azure Portal te verhelpen en de gebruikerstoegang tot Yammer te herstellen:

1.  Open de Azure Active Directory-pagina en selecteer **Enterprise-toepassingen** onder **Beheren** in het linkernavigatiedeelvenster.
3.  Typ **Office 365 Yammer** in het zoekvak en selecteer de naam van de toepassing om instellingen te openen.
4.  Selecteer **Eigenschappen** onder **Beheren** in het linkernavigatiedeelvenster.
5.  De waarde instellen van Ingeschakeld voor gebruikers **Yes**om zich aan **Save** **te melden?**
6.  Meld u opnieuw aan bij Yammer. Het kan nodig zijn om cookies te wissen.

U ook PowerShell-opdrachten uitvoeren om de waarde in te stellen. Zie [de fout 'Sorry, maar we hebben problemen met aanmelden' als u op de Yammer-tegel klikt in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)voor meer informatie. 