---
title: Problemen oplossen met het registreren van Windows-apparaten in Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658873"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d1e9f-102">Problemen oplossen met het registreren van Windows-apparaten in Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="d1e9f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d1e9f-103">Bekijk de onderstaande bronnen om uw probleem nu op te lossen.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d1e9f-104">Enkele veelvoorkomende foutberichten en oplossingsstappen:</span><span class="sxs-lookup"><span data-stu-id="d1e9f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d1e9f-105">**De software kan niet worden geïnstalleerd, 0x80cf4017:** Uw accountcertificaat is verlopen.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d1e9f-106">Download het pakket met de PC-client opnieuw in de intune-beheer console.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d1e9f-107">Raadpleeg deze documentatie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d1e9f-108">**Foutcode 0x801c0003:** De fout kan optreden in de volgende scenario's:</span><span class="sxs-lookup"><span data-stu-id="d1e9f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d1e9f-109">De gebruiker heeft meer apparaten geregistreerd dan de limiet van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d1e9f-110">Bekijk deze documenten om [een apparaat te verwijderen](https://docs.microsoft.com/intune/devices-wipe) of [de limiet voor apparaten te wijzigen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d1e9f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d1e9f-111">' Gebruikers kunnen deelnemen aan een Azure AD ' is ingesteld op ' geen '.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d1e9f-112">Dit instellen op alle of gebruikers selecteren.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-112">Set it to all or select users.</span></span> <span data-ttu-id="d1e9f-113">Raadpleeg [deze documentatie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d1e9f-114">Het apparaat is al ingeschreven door een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d1e9f-115">Als dat het geval is, verwijdert u het apparaat uit de Azure intune-console of verwijdert u het apparaat handmatig en deregistreren voordat u het opnieuw probeert.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d1e9f-116">Het apparaat is Windows 10 voor thuisgebruik.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d1e9f-117">Alleen Windows 10 Pro, Education en Enterprise Sku's kunnen lid worden van Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d1e9f-118">Aanvullende informatiebronnen voor hulp bij het oplossen van het probleem:</span><span class="sxs-lookup"><span data-stu-id="d1e9f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d1e9f-119">Gebruik de portal voor het [oplossen van problemen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) bij het opsporen en oplossen van veelvoorkomende problemen met de inschrijving.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d1e9f-120">Bekijk [dit document](https://docs.microsoft.com/intune/help-desk-operators) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d1e9f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d1e9f-121">Bekijk deze documenten voor een lijst met veelvoorkomende fouten die kunnen worden ingeschreven en opgelost: voor het [oplossen van problemen](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) en het oplossen van [problemen met doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d1e9f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d1e9f-122">[Meer informatie over het registreren van Windows-apparaten in Microsoft intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d1e9f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
