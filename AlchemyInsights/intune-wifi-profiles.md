---
title: Wi-Fi-profielen van Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555004"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="29693-102">Wi-Fi-profielen van Intune</span><span class="sxs-lookup"><span data-stu-id="29693-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="29693-103">Een succesvolle implementatie van Wi-Fi-connectiviteit voor MDM-clients is afhankelijk van een correct geïmplementeerd profiel dat de vereisten van de zakelijke Wi-Fi-infrastructuur weerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="29693-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="29693-104">Zie voor het bekijken van de juiste instellingen voor de clientplatforms die u onderzoekt:</span><span class="sxs-lookup"><span data-stu-id="29693-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="29693-105">Wi-Fi-instellingen toevoegen voor apparaten met Android in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="29693-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="29693-106">Wi-Fi-instellingen toevoegen voor speciale en volledig beheerde apparaten van Android Enterprise in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="29693-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="29693-107">Wi-Fi-instellingen toevoegen voor iOS- en iPadOS-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="29693-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="29693-108">Wi-Fi-instellingen toevoegen voor Windows 10- en nieuwe apparaten in Intune</span><span class="sxs-lookup"><span data-stu-id="29693-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="29693-109">Wi-Fi-instellingen importeren voor Windows-apparaten in Intune</span><span class="sxs-lookup"><span data-stu-id="29693-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="29693-110">**Veelvoorkomende problemen**</span><span class="sxs-lookup"><span data-stu-id="29693-110">**Common Issues**</span></span>

<span data-ttu-id="29693-111">**Ik implementeer een Wi-Fi-profiel dat afhankelijk is van een geïmplementeerd certificaat dat is opgegeven in het Wi-Fi-profiel. De configuratieprofielen vertonen echter een foutstatus.**</span><span class="sxs-lookup"><span data-stu-id="29693-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="29693-112">Controleer of uw apparaat het certificaat heeft ontvangen.</span><span class="sxs-lookup"><span data-stu-id="29693-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="29693-113">Ga in Intune naar **Alle apparaten** en selecteer het apparaat > **apparaatconfiguratie**.</span><span class="sxs-lookup"><span data-stu-id="29693-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="29693-114">Controleer of alle verwachte profielen worden vermeld en in een succesvolle staat.</span><span class="sxs-lookup"><span data-stu-id="29693-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="29693-115">Als u voor een Android-profiel tussentijdse certificaten in uw certificaatketen hebt, controleert u of ze worden geïmplementeerd op Android-apparaten.</span><span class="sxs-lookup"><span data-stu-id="29693-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="29693-116">Als u de certificaatstatus wilt controleren, gaat u naar **Apparaatconfiguratieprofielen**  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="29693-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="29693-117">Als u fouten blijft zien, controleert u de procedures en de secties voor het oplossen van problemen.</span><span class="sxs-lookup"><span data-stu-id="29693-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="29693-118">Zie [Overzicht voor het oplossen van SCEP-certificaatprofielen met Microsoft Intune voor](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="29693-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="29693-119">**Ik heb een Wi-Fi-profiel geïmplementeerd op een apparaat. Intune laat zien dat het succesvol was, maar het apparaat maakt geen verbinding met de Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="29693-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="29693-120">Een succesvolle status betekent dat Intune het profiel heeft geïmplementeerd als geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="29693-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="29693-121">Deze configuraties komen echter mogelijk niet overeen met uw netwerk- en/of verificatievereisten.</span><span class="sxs-lookup"><span data-stu-id="29693-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="29693-122">Voor meer informatie over de geprobeerde verbinding, controleert u logboeken in de infrastructuur- en verificatieservice (op de Wi-Fi Access Point-controller en NPS/Radius-server).</span><span class="sxs-lookup"><span data-stu-id="29693-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="29693-123">Mogelijk moet u samenwerken met uw netwerkinfrastructuurteam of de wi-fi-leverancier van derden om logboeken te verzamelen en te bekijken.</span><span class="sxs-lookup"><span data-stu-id="29693-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>