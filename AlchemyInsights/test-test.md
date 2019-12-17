---
title: Voorwaarden ontbreken in SharePoint Online term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053508"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="eec50-102">BitLocker-versleuteling inschakelen met intune</span><span class="sxs-lookup"><span data-stu-id="eec50-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="eec50-103">InTune Endpoint Protection-beleid kan worden gebruikt voor het configureren van Boitlocker-versleutelingsinstellingen voor Windows-apparaten zoals beschreven in: Windows10 (en latere) instellingen om apparaten te beveiligen met behulp van intune</span><span class="sxs-lookup"><span data-stu-id="eec50-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="eec50-104">U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van MDM-beleid.</span><span class="sxs-lookup"><span data-stu-id="eec50-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="eec50-105">Dit kan invloed hebben op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="eec50-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="eec50-106">Zie de veelgestelde vragen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="eec50-106">See FAQ for more detail.</span></span>


<span data-ttu-id="eec50-107">Veelgestelde  vragen over Q: welke edities van Windows ondersteuning voor apparaatversleuteling met behulp van het Endpoint Protection-beleid?</span><span class="sxs-lookup"><span data-stu-id="eec50-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="eec50-108"> A: de instellingen in intune Endpoint Protection-beleid worden geïmplementeerd met behulp van de BitLocker-CSP.</span><span class="sxs-lookup"><span data-stu-id="eec50-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="eec50-109">Niet alle edities of builds van Windows ondersteunen de BitLocker-CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="eec50-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="eec50-110">Op dit moment Windows-edities: Enterprise; Onderwijs, mobiel, mobiel ondernemen en professioneel (vanaf build 1809) worden ondersteund.</span><span class="sxs-lookup"><span data-stu-id="eec50-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="eec50-111">V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en codeersterkte (XTS-AES-128) zal een beleid met verschillende instellingen automatisch opnieuw versleutelen van het station activeren met de nieuwe instellingen?</span><span class="sxs-lookup"><span data-stu-id="eec50-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="eec50-112">A: Nee.</span><span class="sxs-lookup"><span data-stu-id="eec50-112">A: No.</span></span> <span data-ttu-id="eec50-113">Om de nieuwe cipher instellingen toe te passen moet het station eerst worden gedecodeerd.</span><span class="sxs-lookup"><span data-stu-id="eec50-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="eec50-114">Opmerking voor apparaten die worden ingeschreven met de stuurautomaat de automatische versleuteling die tijdens OOBE optreden wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, waardoor de beleidsinstellingen die kunnen worden gebruikt in plaats van de standaardwaarden van het besturingssysteem</span><span class="sxs-lookup"><span data-stu-id="eec50-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="eec50-115">V als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid wordt deze ontsleuteld wanneer dat beleid wordt verwijderd?</span><span class="sxs-lookup"><span data-stu-id="eec50-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="eec50-116">A: verwijdering van versleuteling gerelateerd beleid leidt niet tot ontsleuteling van de stations die zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="eec50-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="eec50-117">V: Waarom laat het nalevingsbeleid van intune zien dat mijn apparaat geen ' BitLocker ingeschakeld ' heeft, maar wel?</span><span class="sxs-lookup"><span data-stu-id="eec50-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="eec50-118">A: de instelling ' BitLocker ingeschakeld ' in het nalevingsbeleid van intune maakt gebruik van de Windows Device Health Attestation (DHA)-client.</span><span class="sxs-lookup"><span data-stu-id="eec50-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="eec50-119">Deze client meet alleen de apparaatstatus tijdens het opstarten.</span><span class="sxs-lookup"><span data-stu-id="eec50-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="eec50-120">Dus als een apparaat niet opnieuw is opgestart sinds BitLocker-versleuteling is voltooid de DHA-client service wordt BitLocker niet rapporteren als actief.</span><span class="sxs-lookup"><span data-stu-id="eec50-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>