---
title: Ontbrekende termen in SharePoint Online-termenarchief
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766848"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="0d078-102">Bitlocker-versleuteling inschakelen met Intune</span><span class="sxs-lookup"><span data-stu-id="0d078-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="0d078-103">Intune Endpoint Protection Policy kan worden gebruikt om De encryptie-instellingen van Boitlocker voor Windows-apparaten te configureren, zoals beschreven in : Windows10 (en hoger) instellingen om apparaten te beschermen met Behulp van Intune</span><span class="sxs-lookup"><span data-stu-id="0d078-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="0d078-104">U moet zich ervan bewust zijn dat veel nieuwere apparaten met Windows 10 automatische bitlocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van het MDM-beleid.</span><span class="sxs-lookup"><span data-stu-id="0d078-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="0d078-105">Dit kan gevolgen hebben voor de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="0d078-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="0d078-106">Zie veelgestelde vragen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0d078-106">See FAQ for more detail.</span></span>


<span data-ttu-id="0d078-107">FAQ  Q: Welke edities van Windows-ondersteuning apparaat encryptie met behulp van het Endpoint Protection Policy?</span><span class="sxs-lookup"><span data-stu-id="0d078-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="0d078-108"> A: De instellingen in het Intune Endpoint Protection Policy worden geïmplementeerd met de Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="0d078-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="0d078-109">Niet alle edities, noch builds van Windows ondersteunen de Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="0d078-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="0d078-110">Op dit moment Windows Editions: Enterprise; Onderwijs, Mobiel, Mobiel Ondernemen en Professional (vanaf build 1809) worden ondersteund.</span><span class="sxs-lookup"><span data-stu-id="0d078-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="0d078-111">V: Als een apparaat al is versleuteld met Bitlocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en versleutelingssterkte (XTS-AES-128) zal het toepassen van een beleid met verschillende instellingen automatisch leiden tot re-encryptie van het station met de nieuwe instellingen?</span><span class="sxs-lookup"><span data-stu-id="0d078-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="0d078-112">A: Nee.</span><span class="sxs-lookup"><span data-stu-id="0d078-112">A: No.</span></span> <span data-ttu-id="0d078-113">Om de nieuwe cijferinstellingen toe te passen moet het station eerst worden gedecodeerd.</span><span class="sxs-lookup"><span data-stu-id="0d078-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="0d078-114">Opmerking Voor apparaten die zijn ingeschreven bij Autopilot wordt de automatische versleuteling die tijdens OOBE zou optreden, pas geactiveerd nadat het Intune-beleid is geëvalueerd, waardoor de beleidsgebaseerde instellingen kunnen worden gebruikt in plaats van de standaardinstellingen van het besturingssysteem</span><span class="sxs-lookup"><span data-stu-id="0d078-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="0d078-115">V Als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid zal het worden gedecodeerd wanneer dat beleid wordt verwijderd?</span><span class="sxs-lookup"><span data-stu-id="0d078-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="0d078-116">A: Verwijdering van encryptie gerelateerde beleid niet resulteren in decryptie van de stations die zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="0d078-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="0d078-117">V: Waarom laat het intune Compliance-beleid zien dat mijn apparaat geen "Bitlocker Enabled" heeft, maar dat is het wel?</span><span class="sxs-lookup"><span data-stu-id="0d078-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="0d078-118">A: De instelling 'Bitlocker ingeschakeld' in het nalevingsbeleid intune maakt gebruik van de DHA-client (Windows Device Health Attestation).</span><span class="sxs-lookup"><span data-stu-id="0d078-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="0d078-119">Deze client meet alleen de apparaatstatus bij het opstarten.</span><span class="sxs-lookup"><span data-stu-id="0d078-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="0d078-120">Dus als een apparaat niet opnieuw is opgestart sinds bitlocker encryptie is voltooid de DHA client service zal niet bitlocker melden als actief.</span><span class="sxs-lookup"><span data-stu-id="0d078-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>