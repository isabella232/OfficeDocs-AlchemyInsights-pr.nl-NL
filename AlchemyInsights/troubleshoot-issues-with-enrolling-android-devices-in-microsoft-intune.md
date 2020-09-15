---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689949"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="418f1-102">Problemen oplossen met het registreren van Android-apparaten in Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="418f1-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="418f1-103">Bekijk de onderstaande bronnen om uw probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="418f1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="418f1-104">Enkele veelvoorkomende problemen en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="418f1-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="418f1-105">**Fout met niet-versleutelde apparaat in de bedrijfs portal:** Voor nieuwere versies van Android, met name vanaf v 7.0, hebt u een opstartwachtwoord code nodig om te controleren of uw apparaat volledig is versleuteld.</span><span class="sxs-lookup"><span data-stu-id="418f1-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="418f1-106">Veelgebruikte oplossingen zijn om een opstartpincode in te schakelen of het apparaat volledig te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="418f1-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="418f1-107">Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="418f1-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="418f1-108">**Apparaten kunnen niet worden ingecheckt met de intune-service of worden niet in de intune-beheerconsole weergegeven:** Bij sommige Samsung 4,4-en 5,5-apparaten werd de service mogelijk niet gecontroleerd.</span><span class="sxs-lookup"><span data-stu-id="418f1-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="418f1-109">Dit probleem kan drie oplossingen voordoen:</span><span class="sxs-lookup"><span data-stu-id="418f1-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="418f1-110">Open handmatig de app intune Company Portal, waarmee automatisch synchronisatie van apparaten wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="418f1-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="418f1-111">Werk het apparaat bij naar Android 6,0 of hoger.</span><span class="sxs-lookup"><span data-stu-id="418f1-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="418f1-112">Schakel Samsung Smart Manager uit voor het beheren van de intune-bedrijfs portal.</span><span class="sxs-lookup"><span data-stu-id="418f1-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="418f1-113">Bekijk [dit document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="418f1-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="418f1-114">Het **gebruikerslicentie type is ongeldig** of de **gebruikersnaam wordt niet herkend:** de gebruiker moet een INtune-of EMS-licentie toewijzen.</span><span class="sxs-lookup"><span data-stu-id="418f1-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="418f1-115">Bekijk deze documenten om een licentie toe te wijzen via: Office-Beheercentrum of Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="418f1-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="418f1-116">Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:</span><span class="sxs-lookup"><span data-stu-id="418f1-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="418f1-117">Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving.</span><span class="sxs-lookup"><span data-stu-id="418f1-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="418f1-118">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="418f1-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="418f1-119">Bekijk [dit document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die niet voor de inschrijving en oplossing zorgen.</span><span class="sxs-lookup"><span data-stu-id="418f1-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="418f1-120">[Meer informatie over het registreren van Android-apparaten in Microsoft intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="418f1-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
