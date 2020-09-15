---
title: BitLocker-herstelsleutels
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685881"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker-herstelsleutels openen

Wanneer u BitLocker-instellingen configureert voor een beleid voor intune-eindpunten, kunt u definiëren of de BitLocker-herstelinformatie moet worden opgeslagen in azure Active Directory.

Als deze instelling is geconfigureerd, zijn de opgeslagen herstelgegevens zichtbaar voor een intune-beheerder als onderdeel van de apparaat-recordgegevens in de bladweergave van intune-apparaten op twee manieren:

Apparaten – Azure AD-apparaten-> apparaat of apparaten-> alle apparaten-> "apparaat"-> herstelsleutels

Als er ook beheerderstoegang tot het apparaat zelf is, kunt u de herstelsleutel (wachtwoord) bekijken door de volgende opdracht uit te voeren vanaf een opdrachtprompt met verhoogde bevoegdheid:

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
Als het apparaat is versleuteld voordat enrolment in intune is versleuteld, is de herstelsleutel mogelijk gekoppeld aan de ' Microsoft-account ' (MSA) waarmee u zich tijdens het OOBE-proces aanmeldt bij het apparaat. Als dat het geval is,  https://onedrive.live.com/recoverykey moet u de apparaten voor wie de herstelsleutels zijn opgeslagen, weergeven en u hierbij aanmelden.
 
Als het apparaat is versleuteld als gevolg van de configuratie via Groepsbeleid op basis van een domein, kunnen de herstelinformatie in de lokale Active Directory worden opgeslagen.
 

