---
title: Gegevens verwijderen en apparaten wissen van Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439156"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="a62d6-102">Gegevens verwijderen en apparaten wissen van Intune</span><span class="sxs-lookup"><span data-stu-id="a62d6-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="a62d6-103">De acties Device Retire en Device Wipe kunnen worden gebruikt om bedrijfsgegevens te verwijderen die door Intune worden beheerd of om een fabrieksreset uit te voeren en het apparaat terug te sturen naar de standaardinstellingen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="a62d6-104">Meld u aan bij Microsoft 365 Device Management en ga naar **Apparaten**  >  **alle apparaten**.</span><span class="sxs-lookup"><span data-stu-id="a62d6-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="a62d6-105">Selecteer het apparaat dat u wilt wissen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="a62d6-106">Selecteer het type externe veeg die u wilt maken.</span><span class="sxs-lookup"><span data-stu-id="a62d6-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="a62d6-107">Met pensioen gaat alleen organisatorische informatie, terwijl volledige doekjes het apparaat herstellen naar de fabrieksinstellingen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="a62d6-108">Selecteer **Ja** om te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="a62d6-109">Totdat het wissen is voltooid, wordt de actiestatus Apparaat weergegeven als In behandeling met pensioen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="a62d6-110">Nadat de actie is voltooid, ziet u het mobiele apparaat niet meer in de lijst met beheerde apparaten.</span><span class="sxs-lookup"><span data-stu-id="a62d6-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="a62d6-111">**Opmerking** Bedrijfsgegevens kunnen niet worden verwijderd van apparaten die zijn aangesloten bij Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a62d6-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="a62d6-112">Zie Apparaten verwijderen met behulp van [het apparaat wissen, met pensioen en handmatig uitrollen van het apparaat voor](https://docs.microsoft.com/intune/devices-wipe)meer informatie over het effect van de acties Met pensioen gaan en wissen, inclusief wat wordt bewaard en wat wordt verwijderd.</span><span class="sxs-lookup"><span data-stu-id="a62d6-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="a62d6-113">Zie [Alle gegevens van een macOS-apparaat wissen als](https://docs.microsoft.com/intune/device-erase)u alle gegevens van een macOS-apparaat wilt wissen.</span><span class="sxs-lookup"><span data-stu-id="a62d6-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>