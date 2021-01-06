---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768812"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f8ca8-102">BitLocker-versleuteling inschakelen met intune</span><span class="sxs-lookup"><span data-stu-id="f8ca8-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="f8ca8-103">Het beleid voor het intune-endpoint voor beveiliging kan worden gebruikt voor het configureren van BitLocker-versleutelingsinstellingen voor Windows-apparaten.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="f8ca8-104">Zie voor meer informatie de [instellingen van Windows 10 (en later) om apparaten te beschermen met intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="f8ca8-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="f8ca8-105">U dient te beseffen dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen, die wordt geactiveerd zonder de toepassing van MDM-beleid.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f8ca8-106">Dit kan van invloed zijn op de toepassing van beleid als niet-standaardinstellingen zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="f8ca8-107">Zie de volgende veelgestelde vragen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="f8ca8-108">Voor informatie over het oplossen van problemen met BitLocker, raadpleegt u [problemen met BitLocker-beleid in Microsoft intune oplossen](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="f8ca8-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="f8ca8-109">**Veelgestelde vragen**</span><span class="sxs-lookup"><span data-stu-id="f8ca8-109">**FAQ**</span></span>

<span data-ttu-id="f8ca8-110">V: welke versies van Windows ondersteunen apparaatversleuteling met het Endpoint Protection-beleid?</span><span class="sxs-lookup"><span data-stu-id="f8ca8-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="f8ca8-111">A: de instellingen in intune-Endpoint Protection-beleid worden geïmplementeerd met de [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="f8ca8-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="f8ca8-112">Niet alle edities of versies van Windows ondersteunen de BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="f8ca8-113">V: hoe kan BitLocker worden ingeschakeld op apparaten zonder dat de interactie met eindgebruikers is vereist?</span><span class="sxs-lookup"><span data-stu-id="f8ca8-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="f8ca8-114">A: zo lang de noodzakelijke voorwaarden zijn aan te passen, kunt u BitLocker ' stille versleuteling ' inschakelen via intune.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="f8ca8-115">Zie de details van de hardwarevereisten en de voorbeeld beleidsinstellingen voor het inschakelen van de Stille versleuteling in het volgende document: [BitLocker-versleuteling](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)op de achtergrond inschakelen.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="f8ca8-116">V: als een apparaat al met BitLocker is versleuteld met de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en versleutelingssterkte (XTS-AES-128), wordt een beleid toegepast met andere instellingen om het station automatisch opnieuw te versleutelen met de nieuwe instellingen?</span><span class="sxs-lookup"><span data-stu-id="f8ca8-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="f8ca8-117">A: Nee.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-117">A: No.</span></span> <span data-ttu-id="f8ca8-118">Als u de nieuwe versleutelingsinstellingen wilt toepassen, moet het station eerst worden gedecodeerd.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="f8ca8-119">**Opmerking:** Voor apparaten die met auto pilot worden ingeschreven, wordt de automatische versleuteling die zich in OOBE voordoet, niet geactiveerd totdat het intune-beleid wordt geëvalueerd, zodat de instellingen op basis van het beleid kunnen worden gebruikt in plaats van de standaardinstellingen van het besturingssysteem.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="f8ca8-120">V: als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid, wordt deze gedecodeerd wanneer dat beleid wordt verwijderd?</span><span class="sxs-lookup"><span data-stu-id="f8ca8-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="f8ca8-121">A: het verwijderen van het versleutelingsbeleid veroorzaakt geen decodering van de stations die zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="f8ca8-122">V: Waarom wordt in het nalevingsbeleid van intune aangegeven dat mijn apparaat BitLocker niet heeft ingeschakeld, ook niet als dit is?</span><span class="sxs-lookup"><span data-stu-id="f8ca8-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="f8ca8-123">A: de instelling ' BitLocker ingeschakeld ' in het intune-nalevingsbeleid maakt gebruik van de client (DHA) voor Windows-apparaatstatusverklaring.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f8ca8-124">Dit is alleen van toepassing op de status van het apparaat tijdens het opstarten.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="f8ca8-125">Als een apparaat na voltooiing van BitLocker-versleuteling niet opnieuw is opgestart, meldt de DHA client service geen BitLocker als actief.</span><span class="sxs-lookup"><span data-stu-id="f8ca8-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 