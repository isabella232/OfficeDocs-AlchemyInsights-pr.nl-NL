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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="d94ef-102">Toegang tot BitLocker-herstelsleutels</span><span class="sxs-lookup"><span data-stu-id="d94ef-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="d94ef-103">Bij het configureren van BitLocker-instellingen intune Endpoint Protection-beleid, is het mogelijk om te definiëren of BitLocker-herstelgegevens moeten worden opgeslagen in azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d94ef-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="d94ef-104">Als deze instelling is geconfigureerd, moeten de opgeslagen herstelgegevens zichtbaar zijn voor een intune-beheerder als onderdeel van de recordgegevens van het apparaat in de intune-apparaten Blade op twee manieren:</span><span class="sxs-lookup"><span data-stu-id="d94ef-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="d94ef-105">Apparaten-Azure AD-apparaten-> "apparaat" of apparaten-> alle apparaten-> "apparaat"-> herstelsleutels</span><span class="sxs-lookup"><span data-stu-id="d94ef-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="d94ef-106">Als u ook beheerderstoegang tot het apparaat zelf hebt, u de herstelsleutel (wachtwoord) zien door de volgende opdracht uit te voeren vanaf een opdrachtprompt met verhoogde bevoegdheid:</span><span class="sxs-lookup"><span data-stu-id="d94ef-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="d94ef-107">Als het apparaat is versleuteld vóór de inschrijving in intune, kan de herstelsleutel zijn gekoppeld aan de ' Microsoft-account ' (MSA) gebruikt voor aanmelding bij het apparaat tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="d94ef-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="d94ef-108">Als dat het geval is, moet https://onedrive.live.com/recoverykey toegang tot en aanmelden met die MSA de apparaten waarvoor herstelsleutels zijn opgeslagen weergeven.</span><span class="sxs-lookup"><span data-stu-id="d94ef-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="d94ef-109">Als het apparaat is gecodeerd als gevolg van de configuratie via Groepsbeleid op basis van een domein, kunnen de herstelgegevens worden opgeslagen in de lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d94ef-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

