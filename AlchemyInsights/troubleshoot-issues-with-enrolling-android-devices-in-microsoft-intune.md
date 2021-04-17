---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830937"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="b74ae-102">Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b74ae-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="b74ae-103">Bekijk de onderstaande resources om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="b74ae-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b74ae-104">Enkele veelvoorkomende problemen en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="b74ae-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="b74ae-105">**Fout apparaat niet versleuteld in bedrijfsportal:** Voor nieuwere versies van Android, met name vanaf v7.0, is een wachtwoordcode voor opstarten vereist om ervoor te zorgen dat uw apparaat volledig is versleuteld.</span><span class="sxs-lookup"><span data-stu-id="b74ae-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="b74ae-106">Veelgebruikte oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="b74ae-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="b74ae-107">Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b74ae-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="b74ae-108">**Apparaten kunnen niet inchecken met de Intune-service of weergeven als 'Ongezond' in de Intune-beheerconsole:** Sommige Samsung 4.4- en 5.5-apparaten kunnen mogelijk niet inchecken bij de service.</span><span class="sxs-lookup"><span data-stu-id="b74ae-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="b74ae-109">Er zijn drie mogelijke oplossingen voor dit probleem:</span><span class="sxs-lookup"><span data-stu-id="b74ae-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="b74ae-110">Open handmatig de Intune Company Portal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="b74ae-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="b74ae-111">Werk het apparaat bij naar Android 6.0 of hoger.</span><span class="sxs-lookup"><span data-stu-id="b74ae-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="b74ae-112">Schakel Samsung Smart Manager uit om de Intune Company Portal te beheren.</span><span class="sxs-lookup"><span data-stu-id="b74ae-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="b74ae-113">Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="b74ae-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="b74ae-114">**Fout bij gebruikerslicentietype Ongeldig** of Niet-herkende **gebruikersnaam:** De gebruiker moet een Intune- of EMS-licentie krijgen.</span><span class="sxs-lookup"><span data-stu-id="b74ae-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b74ae-115">Controleer deze documenten om een licentie toe te wijzen via: Office-beheercentrum of Azure-portal.</span><span class="sxs-lookup"><span data-stu-id="b74ae-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="b74ae-116">Extra bronnen om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="b74ae-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b74ae-117">Gebruik [Intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten te diagnosticeren en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="b74ae-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b74ae-118">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b74ae-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="b74ae-119">Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elk document voorkomen.</span><span class="sxs-lookup"><span data-stu-id="b74ae-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="b74ae-120">[Meer informatie over het registreren van Android-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="b74ae-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
