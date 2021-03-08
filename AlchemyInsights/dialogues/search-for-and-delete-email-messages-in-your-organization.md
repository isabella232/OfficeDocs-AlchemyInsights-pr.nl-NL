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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523692"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-mailberichten in uw organisatie zoeken en verwijderen

Ga als volgt te werk:

1. Als u geen globale beheerder bent, moet u voor het zoeken naar berichten uw account toevoegen aan de **rollengroep eDiscovery Manager** of de rol **compliancezoekbeheer.** Als u berichten wilt verwijderen, moet u lid worden van de rollengroep **Organisatiebeheer** of de rol Zoeken **en wissen.** Machtigingen voor deze rollen worden toegewezen in het [beveiligings- & compliancecentrum.](https://protection.office.com)
2. [Maak een inhoudszoekactie](https://docs.microsoft.com/office365/securitycompliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.
3. [Maak verbinding met beveiligings & Compliancecentrum PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Als u MFA gebruikt, bekijkt u deze instructies: Verbinding maken met & [Compliancecentrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) met behulp van meervoudige verificatie
4. Het bericht verwijderen: voer de `New-ComplianceSearchAction` cmdlet uit om het bericht te verwijderen. Verwijderde berichten worden verplaatst naar de map Herstelbare items van een gebruiker. Zie stap [3: Het bericht](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization) verwijderen voor een voorbeeldopdracht.
