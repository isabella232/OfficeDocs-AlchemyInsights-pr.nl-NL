---
title: Bitlocker-herstelsleutels
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820281"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="692e5-102">Toegang tot Bitlocker-herstelsleutels</span><span class="sxs-lookup"><span data-stu-id="692e5-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="692e5-103">Bij het configureren van Bitlocker-instellingen Intune Endpoint Protection Policy is het mogelijk om te bepalen of Bitlocker-herstelgegevens moeten worden opgeslagen in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="692e5-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="692e5-104">Als deze instelling is geconfigureerd, moeten de opgeslagen herstelgegevens op twee manieren zichtbaar zijn voor een Intune-beheerder als onderdeel van de apparaatrecordgegevens in het blade Intune Devices:</span><span class="sxs-lookup"><span data-stu-id="692e5-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="692e5-105">Apparaten - Azure AD-apparaten -> 'Device' OR Devices -> All Devices -> 'Device' -> Recovery keys</span><span class="sxs-lookup"><span data-stu-id="692e5-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="692e5-106">Als er ook beheerderstoegang tot het apparaat zelf is, kunt u de herstelsleutel (Wachtwoord) zien door de volgende opdracht uit te voeren vanuit een opdrachtprompt met verhoogde opdracht:</span><span class="sxs-lookup"><span data-stu-id="692e5-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="692e5-107">Als het apparaat is versleuteld vóór de inschrijving in Intune, is de herstelsleutel mogelijk gekoppeld aan het 'Microsoft-account' (MSA) dat is gebruikt om u aan te melden bij het apparaat tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="692e5-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="692e5-108">Als dat het geval was, moet het openen en aanmelden met die MSA de apparaten laten zien waarvoor  https://onedrive.live.com/recoverykey herstelsleutels zijn opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="692e5-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="692e5-109">Als het apparaat is versleuteld als gevolg van configuratie via domeingebaseerd groepsbeleid, worden de herstelgegevens mogelijk opgeslagen in de on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="692e5-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="692e5-110">Als u het endpointbeveiligingsbeleid hebt geconfigureerd voor het opslaan van de herstelsleutel in Azure Active Directory, maar de sleutel voor een specifiek apparaat niet is geüpload, kunt u de upload activeren door de herstelsleutel voor dat apparaat te draaien vanaf de MEM-console.</span><span class="sxs-lookup"><span data-stu-id="692e5-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="692e5-111">Zie [BitLocker-herstelsleutels draaien voor meer informatie.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="692e5-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

