---
title: DLP-regel voor Us Bank Account Number werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005013"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemen met Amerikaanse bankrekeningnummers

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**DLP-problemen met Amerikaanse bankrekeningnummers**

Hebt u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een Amerikaanse **bankrekeningnummer** bevat bij het gebruik van een type DLP-gevoelige informatie in O365? Zo ja, zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.
  
Voor een beleid voor **amerikaanse** bankrekeningnummer dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende gegevens geëvalueerd en moet de regel worden gedetecteerd om de regel te activeren:
  
- **[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cijfers

- **[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 opeenvolgende cijfers.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen Checksum

- **[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Een DLP-beleid is 75% ervan overtuigd dat dit type gevoelige informatie is gedetecteerd als dit binnen een nabijheid van 300 tekens:

  - De normale expressie Regex_usa_bank_account_number inhoud die overeenkomt met het patroon

  - Er wordt een trefwoord Keyword_usa_Bank_Account gevonden.

    In het volgende voorbeeld wordt bijvoorbeeld het beleid voor bankrekeningnummer van de **VS** in gang 78344011

Zie de volgende sectie in  dit artikel voor meer informatie over wat er nodig is voor het detecteren van een Amerikaanse bankrekeningnummer voor uw inhoud: Wat de typen gevoelige informatie voor us [bankrekeningnummer zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: Waar de typen gevoelige informatie naar zoeken met behulp van een ander ingebouwde [gevoelige informatietype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  