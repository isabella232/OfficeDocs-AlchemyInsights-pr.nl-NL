---
title: BitLocker-herstelsleutels
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908810"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Toegang tot BitLocker-herstelsleutels

Bij het configureren van BitLocker-instellingen intune Endpoint Protection-beleid, is het mogelijk om te definiëren of BitLocker-herstelgegevens moeten worden opgeslagen in azure Active Directory.

Als deze instelling is geconfigureerd, moeten de opgeslagen herstelgegevens zichtbaar zijn voor een intune-beheerder als onderdeel van de recordgegevens van het apparaat in de intune-apparaten Blade op twee manieren:

Apparaten-Azure AD-apparaten-> "apparaat" of apparaten-> alle apparaten-> "apparaat"-> herstelsleutels

Als u ook beheerderstoegang tot het apparaat zelf hebt, u de herstelsleutel (wachtwoord) zien door de volgende opdracht uit te voeren vanaf een opdrachtprompt met verhoogde bevoegdheid:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Als het apparaat is versleuteld vóór de inschrijving in intune, kan de herstelsleutel zijn gekoppeld aan de ' Microsoft-account ' (MSA) gebruikt voor aanmelding bij het apparaat tijdens het OOBE-proces. Als dat het geval is, moet https://onedrive.live.com/recoverykey toegang tot en aanmelden met die MSA de apparaten waarvoor herstelsleutels zijn opgeslagen weergeven.
 
Als het apparaat is gecodeerd als gevolg van de configuratie via Groepsbeleid op basis van een domein, kunnen de herstelgegevens worden opgeslagen in de lokale Active Directory.
 

