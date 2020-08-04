---
title: Implementatie van clientverificatiecertificaten oplossen
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555003"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="f92ca-102">Implementatie van clientverificatiecertificaten oplossen</span><span class="sxs-lookup"><span data-stu-id="f92ca-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="f92ca-103">Intune NDES/SCEP en PKCS/PFX Client certificaten profielen profielen worden vaak gebruikt in combinatie met andere profielen types zoals Wifi, VPN, en e-mail om gebruikers te authenticeren om corporate resources.</span><span class="sxs-lookup"><span data-stu-id="f92ca-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="f92ca-104">Wanneer deze profieltypen zijn gekoppeld aan een clientcertificaatprofiel, zijn ze afhankelijk van de succesvolle implementatie van dat profiel.</span><span class="sxs-lookup"><span data-stu-id="f92ca-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="f92ca-105">De eerste infrastructuurinstelling en de bijbehorende configuratie van het clientcertificaatprofiel vereisen vaak probleemoplossing.</span><span class="sxs-lookup"><span data-stu-id="f92ca-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="f92ca-106">Zie voor een stapsgewijze handleiding voor het succesvol instellen van de NDES-connector en richtlijnen voor het oplossen van problemen met de implementatie van certificaten:</span><span class="sxs-lookup"><span data-stu-id="f92ca-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="f92ca-107">Infrastructuur configureren om SCEP te ondersteunen met Intune</span><span class="sxs-lookup"><span data-stu-id="f92ca-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="f92ca-108">Overzicht voor het oplossen van SCEP-certificaatprofielen met Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f92ca-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="f92ca-109">Gebruik de powershell-scripts waarnaar wordt verwezen om uw configuratie te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="f92ca-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="f92ca-110">Zie [Verificatiescripts voor Intune Certificate-connector voor](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)meer informatie .</span><span class="sxs-lookup"><span data-stu-id="f92ca-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="f92ca-111">**Andere veelvoorkomende kwesties**</span><span class="sxs-lookup"><span data-stu-id="f92ca-111">**Other common issues**</span></span>

<span data-ttu-id="f92ca-112">**Wanneer ik de Intune-certificaatconnector op de NDES-connectorserver probeer te installeren, krijg ik het bericht: "Het wachtwoord in het certificaatverzoek kan niet worden geverifieerd. Het kan al gebruikt zijn. Een nieuw wachtwoord aanvragen om met dit verzoek in te dienen."**</span><span class="sxs-lookup"><span data-stu-id="f92ca-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="f92ca-113">Dit bericht betekent dat u de installatie van de certificaatconnector als administrator moet uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="f92ca-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="f92ca-114">In sommige omgevingen moeten de servers waarop het Intune-certificaat wordt uitgevoerd, een proxyserver gebruiken om verbinding te maken met Intune, zodat de Certificate Connector een proxy moet gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f92ca-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="f92ca-115">In sommige gevallen negeert de NDES-connector de geconfigureerde proxy-instellingen en is het mogelijk dat de proxy-instellingen tijdens het uitvoeren in de beveiligingscontext van LocalSystem moeten worden geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="f92ca-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="f92ca-116">De oplossing is om Internet Explorer als SYSTEEM uit te voeren en een proxy in IE te configureren.</span><span class="sxs-lookup"><span data-stu-id="f92ca-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="f92ca-117">Na een herstart van de Intune Connector Service maakt de NDES Connector verbinding met Intune.</span><span class="sxs-lookup"><span data-stu-id="f92ca-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="f92ca-118">**Gebruikersapparaten ontvangen geen SCEP-certificaten meer van NDES.**</span><span class="sxs-lookup"><span data-stu-id="f92ca-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="f92ca-119">Het is mogelijk dat het certificaat voor clientverificatie dat is afgegeven aan de NDES-server en is opgegeven tijdens de installatie van de NDES-connector, is verlopen of ontbreekt.</span><span class="sxs-lookup"><span data-stu-id="f92ca-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="f92ca-120">Ga als een oplossing voor:</span><span class="sxs-lookup"><span data-stu-id="f92ca-120">To resolve:</span></span> 
 
1. <span data-ttu-id="f92ca-121">Verwijder de NDES-connector.</span><span class="sxs-lookup"><span data-stu-id="f92ca-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="f92ca-122">Gebruik deze gegevens om een nieuw certificaat voor clientverificatie of serververificatie aan te vragen:</span><span class="sxs-lookup"><span data-stu-id="f92ca-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="f92ca-123">Onderwerpnaam: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="f92ca-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="f92ca-124">Onderwerp alternatieve naam (beide zijn vereist): DNS=externe fqdn, DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="f92ca-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="f92ca-125">Installeer de NDES-connector opnieuw met het nieuwe certificaat.</span><span class="sxs-lookup"><span data-stu-id="f92ca-125">Reinstall the NDES connector with the new certificate.</span></span>