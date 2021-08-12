---
title: E-mailberichten in uw organisatie zoeken en verwijderen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948878"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-mailberichten in uw organisatie zoeken en verwijderen

Volg deze stappen:

1. Als u geen globale beheerder bent, moet u als u wilt zoeken naar berichten uw account worden toegevoegd aan de rollengroep **eDiscovery Manager** of **compliancezoekbeheerrol.** Als u berichten wilt verwijderen, moet u lid worden van de rollengroep **Organisatiebeheer** of de rol **zoeken en verwijderen.** Machtigingen voor deze rollen worden toegewezen in het [beveiligings- & compliancecentrum.](https://protection.office.com)
2. [Maak een inhoudszoekactie](https://docs.microsoft.com/office365/securitycompliance/content-search) om het bericht te vinden dat u wilt verwijderen.
3. [Verbinding maken met Beveiligings- en compliancecentrum van Powershell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Als u MFA gebruikt, bekijkt u deze instructies: [Verbinding maken Security & Compliance Center PowerShell met meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Het bericht verwijderen: voer de `New-ComplianceSearchAction` cmdlet uit om het bericht te verwijderen. Verwijderde berichten worden verplaatst naar de map Herstelbare items van een gebruiker. Zie Stap [3: Het bericht verwijderen](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization) voor een voorbeeldopdracht.
