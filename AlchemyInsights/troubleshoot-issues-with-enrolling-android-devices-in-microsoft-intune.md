---
title: Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708993"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="3f251-102">Problemen oplossen met het registreren van Android-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3f251-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="3f251-103">Bekijk de onderstaande bronnen om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="3f251-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3f251-104">Enkele veelvoorkomende problemen en oplossingen:</span><span class="sxs-lookup"><span data-stu-id="3f251-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="3f251-105">**Fout in bedrijfsportal apparaat niet versleuteld:** Voor nieuwere versies van Android, met name die met v7.0, is een opstartcode vereist om ervoor te zorgen dat uw apparaat volledig is versleuteld.</span><span class="sxs-lookup"><span data-stu-id="3f251-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="3f251-106">Veelvoorkomende oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="3f251-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="3f251-107">Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="3f251-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="3f251-108">**Apparaten kunnen niet worden inchecken met de Intune-service** of worden weergegeven als Niet-in orde in de Intune-beheerconsole: Sommige Samsung 4.4- en 5.5-apparaten checken mogelijk niet in bij de service.</span><span class="sxs-lookup"><span data-stu-id="3f251-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="3f251-109">Er zijn drie mogelijke oplossingen voor dit probleem:</span><span class="sxs-lookup"><span data-stu-id="3f251-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="3f251-110">Open handmatig de Intune-bedrijfsportal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="3f251-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="3f251-111">Werk het apparaat bij naar Android 6.0 of hoger.</span><span class="sxs-lookup"><span data-stu-id="3f251-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="3f251-112">Schakel Samsung Smart Manager uit voor het beheren van de Intune-bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="3f251-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="3f251-113">Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze problemen en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="3f251-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="3f251-114">**Fout: gebruikerslicentietype ongeldig** of gebruikersnaam **niet herkend:** aan de gebruiker moet een Intune- of EMS-licentie worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="3f251-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3f251-115">Bekijk deze documenten om een licentie toe te wijzen via: Office-beheercentrum of Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3f251-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="3f251-116">Aanvullende bronnen om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="3f251-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3f251-117">Gebruik [intune Troubleshooting Portal om](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) veelvoorkomende registratiefouten op te sporen en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="3f251-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3f251-118">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="3f251-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="3f251-119">Bekijk [dit document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) voor een lijst met veelvoorkomende fouten die inschrijving en oplossingen voor elke fout verhinderen.</span><span class="sxs-lookup"><span data-stu-id="3f251-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="3f251-120">[Meer informatie over het registreren van Android-apparaten in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="3f251-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
