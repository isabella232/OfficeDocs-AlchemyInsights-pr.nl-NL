---
title: Gegevens verwijderen en apparaten wissen uit Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416308"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="bdd08-102">Gegevens verwijderen en apparaten wissen uit Intune</span><span class="sxs-lookup"><span data-stu-id="bdd08-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="bdd08-103">Met de acties apparaat buiten gebruik stellen en apparaat wissen kunnen bedrijfsgegevens die beheerd worden door Intune verwijderd worden of de fabrieksinstellingen opnieuw ingesteld worden.</span><span class="sxs-lookup"><span data-stu-id="bdd08-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="bdd08-104">Meld je aan in Microsoft 365-apparaatbeheer en ga naar **Apparaten** > **Alle apparaten**.</span><span class="sxs-lookup"><span data-stu-id="bdd08-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="bdd08-105">Selecteer het apparaat dat je wilt wissen.</span><span class="sxs-lookup"><span data-stu-id="bdd08-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="bdd08-106">Selecteer het type wissen van op afstand dat je wilt uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="bdd08-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="bdd08-107">Buiten gebruik stellen verwijdert enkel informatie van de organisatie. Volledig wissen herstelt de fabrieksinstellingen op het apparaat. </span><span class="sxs-lookup"><span data-stu-id="bdd08-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="bdd08-108">Selecteer **Ja** om te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="bdd08-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="bdd08-109">Totdat wissen voltooid is wordt de status van het apparaat als *buiten gebruik stellen in behandeling* weergegeven.</span><span class="sxs-lookup"><span data-stu-id="bdd08-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="bdd08-110">Nadat de actie voltooid is wordt het mobiele apparaat niet meer in de lijst van beheerde apparaten weergegeven.</span><span class="sxs-lookup"><span data-stu-id="bdd08-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="bdd08-111">Bedrijfsgegevens kunnen niet verwijderd worden uit apparaten die aan Azure AD toegevoegd zijn.</span><span class="sxs-lookup"><span data-stu-id="bdd08-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="bdd08-112">Voor een volledig overzicht van de gevolgen van de acties buiten gebruik stellen en wissen, inclusief wat behouden wordt en wat verwijderd wordt, zie de volgende documentatie:</span><span class="sxs-lookup"><span data-stu-id="bdd08-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="bdd08-113">[Apparaten verwijderen met wissen, buiten gebruik stellen of het apparaat manueel uitschrijven](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="bdd08-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="bdd08-114">Hoe enkel bedrijfsgegevens wissen uit Intune-beheerde apps</span><span class="sxs-lookup"><span data-stu-id="bdd08-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="bdd08-115">[Alle gegevens wissen uit een macOS-apparaat](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="bdd08-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>