---
title: VPN-gerelateerde problemen
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554971"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="ad9e5-102">VPN-gerelateerde problemen</span><span class="sxs-lookup"><span data-stu-id="ad9e5-102">VPN related issues</span></span>

<span data-ttu-id="ad9e5-103">Succesvolle implementatie van VPN-connectiviteit voor MDM-clients is afhankelijk van een geïmplementeerd profiel dat de vereisten van de VPN-infrastructuur correct weergeeft.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="ad9e5-104">Zie voor de juiste instellingen voor de clientplatforms die u onderzoekt:</span><span class="sxs-lookup"><span data-stu-id="ad9e5-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="ad9e5-105">Windows 10- en Windows-holografische apparaatinstellingen om VPN-verbindingen toe te voegen met Intune</span><span class="sxs-lookup"><span data-stu-id="ad9e5-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="ad9e5-106">VPN-instellingen toevoegen op iOS- en iPadOS-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ad9e5-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="ad9e5-107">Instellingen voor Android-apparaten om VPN in Intune te configureren</span><span class="sxs-lookup"><span data-stu-id="ad9e5-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="ad9e5-108">VPN-instellingen toevoegen op macOS-apparaten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ad9e5-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="ad9e5-109">Als uw VPN-profiel verificatie op basis van certificaten gebruikt, controleert u of de hoofdcertificaat- en clientverificatiecertificaatprofielen die aan het VPN-profiel zijn gekoppeld, met succes worden geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="ad9e5-110">**Veelvoorkomende problemen**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-110">**Common Issues**</span></span>

<span data-ttu-id="ad9e5-111">**Ik heb een VPN-profiel geïmplementeerd op een apparaat. Intune laat zien dat het succesvol was, maar het apparaat maakt geen verbinding met de VPN.**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="ad9e5-112">Een succesvolle status betekent dat Intune het profiel heeft geïmplementeerd als geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="ad9e5-113">Deze configuraties komen echter mogelijk niet overeen met uw netwerk- en/of verificatievereisten.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="ad9e5-114">Bekijk logboeken in de infrastructuur- en verificatieservice (op de VPN-server en NPS/Radius-server) voor meer informatie over de geprobeerde verbinding.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="ad9e5-115">Mogelijk moet u samenwerken met uw netwerkinfrastructuurteam of de VPN-leverancier van derden om logboeken te verzamelen en te bekijken.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="ad9e5-116">**Wanneer ik een aangepaste VPN voor iOS configureer, wordt de VPN-functie per app niet beschikbaar gesteld.**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="ad9e5-117">Per-app VPN voor iOS-apparaten in Intune is momenteel beschikbaar voor een specifieke lijst van providers en partners, die ook moeten voldoen aan de certificaatvoorwaarden voordat u een VPN per app configureert.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="ad9e5-118">Zie [VPN (Virtual Private Network) instellen per app Virtual Private Network (VPN) instellen voor iOS/iPadOS-apparaten in Intune.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="ad9e5-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="ad9e5-119">Zie [VPN-profielen maken om verbinding te maken met VPN-servers in Intune voor](https://docs.microsoft.com/intune/vpn-settings-configure)meer informatie over alle VPN-verbindingstypen in Intune.</span><span class="sxs-lookup"><span data-stu-id="ad9e5-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="ad9e5-120">**iOS On-Demand VPN wordt niet geactiveerd wanneer een geconfigureerd domein wordt geopend**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="ad9e5-121">Als u automatische VPN-instellingen wilt testen, stelt u de volgende waarden in:</span><span class="sxs-lookup"><span data-stu-id="ad9e5-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="ad9e5-122">Ik wil het volgende doen: **Elke verbindingspoging evalueren**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="ad9e5-123">Kiezen of u verbinding wilt maken: **maak verbinding indien nodig**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="ad9e5-124">Wanneer gebruikers toegang krijgen tot deze domeinen: **target** *doeldomeinnaam*</span><span class="sxs-lookup"><span data-stu-id="ad9e5-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="ad9e5-125">Als de bovenstaande configuratie niet is geslaagd, voegt u het volgende element toe:</span><span class="sxs-lookup"><span data-stu-id="ad9e5-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="ad9e5-126">Wanneer deze URL onbereikbaar is, force connect the VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="ad9e5-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>