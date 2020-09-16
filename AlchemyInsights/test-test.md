---
title: Ontbrekende voorwaarden in het SharePoint Online-Termenarchief
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750446"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ba47e-102">BitLocker-versleuteling inschakelen met intune</span><span class="sxs-lookup"><span data-stu-id="ba47e-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="ba47e-103">Het beleid voor het intune-endpoint voor beveiliging kan worden gebruikt voor het configureren van Boitlocker versleutelingsinstellingen voor Windows-apparaten, zoals beschreven in de Windows 10-(en latere) instellingen om apparaten te beschermen met intune.</span><span class="sxs-lookup"><span data-stu-id="ba47e-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="ba47e-104">U dient te beseffen dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van MDM-beleid.</span><span class="sxs-lookup"><span data-stu-id="ba47e-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ba47e-105">Dit kan van invloed zijn op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="ba47e-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="ba47e-106">Zie Veelgestelde vragen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ba47e-106">See FAQ for more detail.</span></span>


<span data-ttu-id="ba47e-107">Veelgestelde vragen   : welke edities van Windows ondersteuning bieden voor apparaatversleuteling met het Endpoint Protection-beleid?</span><span class="sxs-lookup"><span data-stu-id="ba47e-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="ba47e-108"> A: de instellingen in intune-Endpoint Protection-beleid worden geïmplementeerd met de BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="ba47e-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="ba47e-109">Niet alle edities en versies van Windows ondersteunen de BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="ba47e-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="ba47e-110">Op dit moment Windows-edities: Enterprise; Education, Mobile, Mobile Enterprise en Professional (vanaf build 1809 en later) worden ondersteund.</span><span class="sxs-lookup"><span data-stu-id="ba47e-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="ba47e-111">V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en cipher vastheid (XTS-AES-128), wordt het toepassen van een beleid waarbij verschillende instellingen worden gebruikt, automatisch opnieuw versleutelen met de nieuwe instellingen?</span><span class="sxs-lookup"><span data-stu-id="ba47e-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="ba47e-112">A: Nee.</span><span class="sxs-lookup"><span data-stu-id="ba47e-112">A: No.</span></span> <span data-ttu-id="ba47e-113">Om de nieuwe instellingen voor Cipher toe te passen, moet het station eerst worden gedecodeerd.</span><span class="sxs-lookup"><span data-stu-id="ba47e-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="ba47e-114">Opmerking voor apparaten die worden geregistreerd met auto pilot de automatische versleuteling die zich in OOBE voordoet, wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, zodat de beleidsinstellingen die kunnen worden gebruikt in plaats van de standaardinstellingen voor het besturingssysteem worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="ba47e-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="ba47e-115">V als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid wordt deze gedecodeerd wanneer dat beleid wordt verwijderd?</span><span class="sxs-lookup"><span data-stu-id="ba47e-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="ba47e-116">A: het verwijderen van een beleids versleuteling heeft geen invloed op de decodering van de stations die zijn geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="ba47e-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="ba47e-117">V: Waarom wordt in het nalevingsbeleid van intune aangegeven dat mijn apparaat geen ' BitLocker ingeschakeld ' bevat, maar het is?</span><span class="sxs-lookup"><span data-stu-id="ba47e-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="ba47e-118">A: de instelling ' BitLocker ingeschakeld ' in het intune-nalevingsbeleid maakt gebruik van de client (DHA) voor Windows-apparaatstatusverklaring.</span><span class="sxs-lookup"><span data-stu-id="ba47e-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ba47e-119">Dit is alleen van toepassing op de status van het apparaat tijdens het opstarten.</span><span class="sxs-lookup"><span data-stu-id="ba47e-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="ba47e-120">Als een apparaat niet opnieuw is opgestart sinds de BitLocker-versleuteling werd voltooid, wordt BitLocker niet door de DHA-client gerapporteerd als actief.</span><span class="sxs-lookup"><span data-stu-id="ba47e-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>