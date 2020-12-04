---
title: Microsoft intune-beveiligings lijnen gebruiken om Windows 10-apparaten te configureren
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573402"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="b7a9f-102">Microsoft intune-beveiligings lijnen gebruiken om Windows 10-apparaten te configureren</span><span class="sxs-lookup"><span data-stu-id="b7a9f-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="b7a9f-103">InTune-beveiligings basislijns helpen gebruikers en apparaten te beschermen.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b7a9f-104">Met behulp van beveiligings lijnen voor Windows-instellingen worden vooraf geconfigureerde groepen gebruikt om een bekende groep instellingen en standaardwaarden die worden aanbevolen door de relevante beveiligings teams toe te passen.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b7a9f-105">Als u een beveiligings basislijn profiel maakt in intune, maakt u een sjabloon met meerdere apparaatconfiguratie-profielen.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b7a9f-106">Wanneer u beveiligings basislijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten die worden uitgevoerd op Windows 10 of later.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="b7a9f-107">Voorbeeld van MDM-beveiliging (1) wordt BitLocker voor verwisselbare schijven niet automatisch ingeschakeld, (2) het wachtwoord voor het ontgrendelen van een apparaat vereist en (3) basisverificatie uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="b7a9f-108">Wanneer een standaardwaarde niet werkt voor uw omgeving, past u de basislijn aan zodat u de gewenste instellingen kunt toepassen.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b7a9f-109">Met behulp van beveiligings lijnen voor beveiliging kunt u ook een end-to-end beveiligde werkstroom maken in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b7a9f-110">Hier volgen enkele voordelen:</span><span class="sxs-lookup"><span data-stu-id="b7a9f-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="b7a9f-111">Een beveiligings basislijn bevat de aanbevolen procedures en aanbevelingen voorinstellingen die van invloed zijn op de beveiliging.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b7a9f-112">Aangezien intune-partners met het Windows-beveiligingsteam basislijnen voor groepsbeleidsregels maken, zijn deze aanbevelingen gebaseerd op een ononderbroken richtlijn en een uitgebreide ervaring.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="b7a9f-113">Als u niet bekend bent met intune en u niet zeker weet waar u moet beginnen, kunt u met behulp van beveiligings lijnen snel een veilig profiel maken en implementeren.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="b7a9f-114">Als u momenteel een Groepsbeleid gebruikt, wordt de migratie naar intune voor beheerdoeleinden veel eenvoudiger gemaakt met behulp van beveiligings lijnen, omdat ze zijn ingebouwd in intune en de functies voor het beheren van de gesneden Edge bevatten.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="b7a9f-115">Zie [Windows-beveiligings lijnen](https://go.microsoft.com/fwlink/?linkid=2141503) en [beheer van mobiele apparaten](https://go.microsoft.com/fwlink/?linkid=2141701)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b7a9f-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>