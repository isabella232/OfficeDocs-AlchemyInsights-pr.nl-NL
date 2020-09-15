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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="56c3d-102">BitLocker-herstelsleutels openen</span><span class="sxs-lookup"><span data-stu-id="56c3d-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="56c3d-103">Wanneer u BitLocker-instellingen configureert voor een beleid voor intune-eindpunten, kunt u definiëren of de BitLocker-herstelinformatie moet worden opgeslagen in azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="56c3d-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="56c3d-104">Als deze instelling is geconfigureerd, zijn de opgeslagen herstelgegevens zichtbaar voor een intune-beheerder als onderdeel van de apparaat-recordgegevens in de bladweergave van intune-apparaten op twee manieren:</span><span class="sxs-lookup"><span data-stu-id="56c3d-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="56c3d-105">Apparaten – Azure AD-apparaten-> apparaat of apparaten-> alle apparaten-> "apparaat"-> herstelsleutels</span><span class="sxs-lookup"><span data-stu-id="56c3d-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="56c3d-106">Als er ook beheerderstoegang tot het apparaat zelf is, kunt u de herstelsleutel (wachtwoord) bekijken door de volgende opdracht uit te voeren vanaf een opdrachtprompt met verhoogde bevoegdheid:</span><span class="sxs-lookup"><span data-stu-id="56c3d-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="56c3d-107">Als het apparaat is versleuteld voordat enrolment in intune is versleuteld, is de herstelsleutel mogelijk gekoppeld aan de ' Microsoft-account ' (MSA) waarmee u zich tijdens het OOBE-proces aanmeldt bij het apparaat.</span><span class="sxs-lookup"><span data-stu-id="56c3d-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="56c3d-108">Als dat het geval is,  https://onedrive.live.com/recoverykey moet u de apparaten voor wie de herstelsleutels zijn opgeslagen, weergeven en u hierbij aanmelden.</span><span class="sxs-lookup"><span data-stu-id="56c3d-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="56c3d-109">Als het apparaat is versleuteld als gevolg van de configuratie via Groepsbeleid op basis van een domein, kunnen de herstelinformatie in de lokale Active Directory worden opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="56c3d-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

