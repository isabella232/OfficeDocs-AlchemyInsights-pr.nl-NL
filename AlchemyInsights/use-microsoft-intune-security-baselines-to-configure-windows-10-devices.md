---
title: De beveiligingsbasislijnen van Microsoft Intune gebruiken om Windows 10-apparaten te configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693415"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="9cddf-102">De beveiligingsbasislijnen van Microsoft Intune gebruiken voor het configureren van Windows 10-apparaten</span><span class="sxs-lookup"><span data-stu-id="9cddf-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="9cddf-103">Intune-beveiligingsbasislijnen helpen gebruikers en apparaten te beschermen.</span><span class="sxs-lookup"><span data-stu-id="9cddf-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="9cddf-104">Beveiligingsbasislijnen zijn vooraf geconfigureerde groepen in Windows-instellingen die worden gebruikt voor het toepassen van een bekende groep instellingen en standaardwaarden die worden aanbevolen door de relevante beveiligingsteams.</span><span class="sxs-lookup"><span data-stu-id="9cddf-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="9cddf-105">Door een beveiligingsbasislijnprofiel te maken in Intune, maakt u een sjabloon die uit meerdere apparaatconfiguratieprofielen bestaat.</span><span class="sxs-lookup"><span data-stu-id="9cddf-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="9cddf-106">Wanneer u beveiligingsbasislijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten met Windows 10 of nieuwere versies.</span><span class="sxs-lookup"><span data-stu-id="9cddf-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="9cddf-107">Zo schakelt de beveiligingsbasislijn van Microsoft Mobile Device Management (MDM) automatisch (1) BitLocker in voor verwisselbare stations, (2) is het wachtwoord vereist voor het ontgrendelen van een apparaat en (3) worden basisverificatie uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="9cddf-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="9cddf-108">Als een standaardwaarde niet werkt voor uw omgeving, kunt u de basislijn aanpassen om de instellingen toe te passen die u nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="9cddf-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="9cddf-109">Beveiligingsbasislijnen helpen ook bij het tot stand brengen van een end-to-end veilige werkstroom in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9cddf-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="9cddf-110">Hier volgen enkele voordelen van deze functionaliteit:</span><span class="sxs-lookup"><span data-stu-id="9cddf-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="9cddf-111">Een basislijn voor beveiliging bevat de aanbevolen procedures en aanbevelingen voor instellingen die van invloed zijn op de beveiliging.</span><span class="sxs-lookup"><span data-stu-id="9cddf-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="9cddf-112">Omdat Intune partners met het Windows-beveiligingsteam basislijnen voor groepsbeleid maakt, zijn deze aanbevelingen gebaseerd op een betrouwbare begeleiding en uitgebreide ervaring.</span><span class="sxs-lookup"><span data-stu-id="9cddf-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="9cddf-113">Als Intune nieuw voor u is en niet zeker weet waar u moet beginnen, kunt u met behulp van beveiligingsbasislijnen snel een beveiligd profiel maken en implementeren.</span><span class="sxs-lookup"><span data-stu-id="9cddf-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="9cddf-114">Als u momenteel een groepsbeleid gebruikt, is een migratie naar Intune voor beheerdoeleinden veel gemakkelijker met beveiligingsbasislijnen, omdat deze beveiligingsbasislijnen zijn ingebouwd in Intune en geavanceerde beheermogelijkheden bevatten.</span><span class="sxs-lookup"><span data-stu-id="9cddf-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="9cddf-115">Zie windows-beveiligingsbasislijnen en [Mobile Device Management voor meer informatie.](https://docs.microsoft.com/windows/client-management/mdm/) [](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="9cddf-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>