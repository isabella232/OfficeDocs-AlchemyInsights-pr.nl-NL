---
title: Data Provider-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908705"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="51dd8-102">BitLocker-versleuteling inschakelen met intune</span><span class="sxs-lookup"><span data-stu-id="51dd8-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="51dd8-103">InTune Endpoint Protection-beleid kan worden gebruikt voor het configureren van BitLocker-versleutelingsinstellingen voor Windows-apparaten.</span><span class="sxs-lookup"><span data-stu-id="51dd8-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="51dd8-104">Zie voor meer informatie [instellingen voor Windows 10 (en hoger) om apparaten te beveiligen met intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="51dd8-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="51dd8-105">U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen, die wordt geactiveerd zonder de toepassing van MDM-beleid.</span><span class="sxs-lookup"><span data-stu-id="51dd8-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="51dd8-106">Dit kan invloed hebben op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="51dd8-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="51dd8-107">Zie de volgende veelgestelde vragen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="51dd8-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="51dd8-108">Zie [problemen met BitLocker-beleid in Microsoft intune oplossen](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)voor meer informatie over het oplossen van problemen met BitLocker.</span><span class="sxs-lookup"><span data-stu-id="51dd8-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="51dd8-109">**Veelgestelde vragen**</span><span class="sxs-lookup"><span data-stu-id="51dd8-109">**FAQ**</span></span>

 <span data-ttu-id="51dd8-110">V: welke edities van Windows ondersteuning voor apparaatversleuteling met behulp van het Endpoint Protection-beleid?</span><span class="sxs-lookup"><span data-stu-id="51dd8-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="51dd8-111">A: de instellingen in intune Endpoint Protection-beleid worden geïmplementeerd met behulp van de [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="51dd8-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="51dd8-112">Niet alle edities of builds van Windows ondersteunen de BitLocker-CSP.</span><span class="sxs-lookup"><span data-stu-id="51dd8-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="51dd8-113">Op dit moment worden de volgende Windows-edities ondersteund: Enterprise, education, Mobile, Mobile Enterprise en Professional (build 1809 en hoger).</span><span class="sxs-lookup"><span data-stu-id="51dd8-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="51dd8-114">V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en codeersterkte (XTS-AES-128), zal een beleid met verschillende instellingen automatisch opnieuw versleutelen van het station activeren met de nieuwe instellingen?</span><span class="sxs-lookup"><span data-stu-id="51dd8-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="51dd8-115">A: Nee.</span><span class="sxs-lookup"><span data-stu-id="51dd8-115">A: No.</span></span> <span data-ttu-id="51dd8-116">Als u de nieuwe coderingsinstellingen wilt toepassen, moet het station eerst worden ontsleuteld.</span><span class="sxs-lookup"><span data-stu-id="51dd8-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="51dd8-117">**Opmerking:** Voor apparaten die worden ingeschreven met Autopilot, wordt de automatische versleuteling die tijdens OOBE optreden wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, waardoor de op beleid gebaseerde instellingen kunnen worden gebruikt in plaats van de standaardwaarden van het besturingssysteem.</span><span class="sxs-lookup"><span data-stu-id="51dd8-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="51dd8-118">V: als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid, wordt deze ontsleuteld wanneer dat beleid wordt verwijderd?</span><span class="sxs-lookup"><span data-stu-id="51dd8-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="51dd8-119">A: het verwijderen van beleid met betrekking tot versleuteling leidt niet tot ontsleuteling van de stations die zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="51dd8-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="51dd8-120">V: Waarom wordt in het nalevingsbeleid van intune weergegeven dat BitLocker niet is ingeschakeld op mijn apparaat, ook al is het?</span><span class="sxs-lookup"><span data-stu-id="51dd8-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="51dd8-121">A: de instelling ' BitLocker ingeschakeld ' in het nalevingsbeleid van intune maakt gebruik van de Windows Device Health Attestation (DHA)-client.</span><span class="sxs-lookup"><span data-stu-id="51dd8-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="51dd8-122">Deze client meet alleen de apparaatstatus tijdens het opstarten.</span><span class="sxs-lookup"><span data-stu-id="51dd8-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="51dd8-123">Dus als een apparaat niet opnieuw is opgestart sinds BitLocker-versleuteling is voltooid, de DHA-client service wordt BitLocker niet rapporteren als actief.</span><span class="sxs-lookup"><span data-stu-id="51dd8-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 