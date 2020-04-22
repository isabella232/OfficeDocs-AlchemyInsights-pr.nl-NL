---
title: Problemen met inschrijvende Android-apparaten in Microsoft Intune oplossen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759615"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="63475-102">Problemen met inschrijvende Android-apparaten in Microsoft Intune oplossen</span><span class="sxs-lookup"><span data-stu-id="63475-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="63475-103">Bekijk de onderstaande bronnen om het probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="63475-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="63475-104">Enkele veelvoorkomende problemen en stappen voor het oplossen van oplossingen:</span><span class="sxs-lookup"><span data-stu-id="63475-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="63475-105">**Apparaat niet versleutelde fout in bedrijfsportal:** Nieuwere versies van Android, met name te beginnen met v7.0, vereisen een opstartcode om ervoor te zorgen dat uw apparaat volledig is versleuteld.</span><span class="sxs-lookup"><span data-stu-id="63475-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="63475-106">Veelvoorkomende oplossingen zijn het inschakelen van een opstartpin of het volledig versleutelen van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="63475-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="63475-107">Bekijk [dit document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="63475-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="63475-108">**Apparaten kunnen niet inchecken met de Intune-service of worden weergegeven als 'Niet in orde' in de Intune-beheerconsole:** Sommige Samsung 4.4- en 5.5-apparaten kunnen niet inchecken in de service.</span><span class="sxs-lookup"><span data-stu-id="63475-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="63475-109">Er zijn 3 mogelijke oplossingen voor dit probleem:</span><span class="sxs-lookup"><span data-stu-id="63475-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="63475-110">Open handmatig de Intune Company Portal-app, waarmee automatisch een apparaatsynchronisatie wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="63475-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="63475-111">Werk het apparaat bij naar Android 6.0 of hoger.</span><span class="sxs-lookup"><span data-stu-id="63475-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="63475-112">Schakel Samsung Smart Manager uit om de Intune Company Portal te beheren.</span><span class="sxs-lookup"><span data-stu-id="63475-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="63475-113">Bekijk [dit document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) voor meer informatie over deze kwesties en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="63475-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="63475-114">**Ongeldig type gebruikerslicentie** of **gebruikersnaam niet-herkende fout:** de gebruiker moet een Intune- of EMS-licentie toegewezen krijgen.</span><span class="sxs-lookup"><span data-stu-id="63475-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="63475-115">Controleer deze documenten om een licentie toe te wijzen via: Office Admin Center of Azure portal.</span><span class="sxs-lookup"><span data-stu-id="63475-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="63475-116">Aanvullende bronnen om uw probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="63475-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="63475-117">Gebruik [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) om veelvoorkomende inschrijvingsfouten te diagnosticeren en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="63475-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="63475-118">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="63475-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="63475-119">Controleer [dit document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) op een lijst met veelvoorkomende fouten die inschrijving en resoluties voor elke instelling voorkomen.</span><span class="sxs-lookup"><span data-stu-id="63475-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="63475-120">[Meer informatie over het inschrijven van Android-apparaten in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="63475-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
