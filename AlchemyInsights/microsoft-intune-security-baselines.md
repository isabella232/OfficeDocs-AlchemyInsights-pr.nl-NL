---
title: Gebruik Microsoft Intune beveiligingslijnlijnen om Windows 10 configureren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793700"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="f579d-102">Gebruik Microsoft Intune beveiligingslijnlijnen om Windows 10 configureren</span><span class="sxs-lookup"><span data-stu-id="f579d-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="f579d-103">Intune-beveiligingslijnlijnen helpen gebruikers en apparaten te beveiligen.</span><span class="sxs-lookup"><span data-stu-id="f579d-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f579d-104">Beveiligingslijnlijnen zijn Windows vooraf geconfigureerde groepen die worden gebruikt om een bekende groep instellingen en standaardwaarden toe te passen die worden aanbevolen door de relevante beveiligingsteams.</span><span class="sxs-lookup"><span data-stu-id="f579d-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f579d-105">Door een beveiligingslijnprofiel te maken in Intune, maakt u een sjabloon die bestaat uit meerdere apparaatconfiguratieprofielen.</span><span class="sxs-lookup"><span data-stu-id="f579d-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f579d-106">Wanneer u beveiligingslijnlijnen implementeert voor groepen gebruikers of apparaten, worden de instellingen toegepast op apparaten die op Windows 10 of hoger worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="f579d-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="f579d-107">De beveiligingslijn voor Microsoft Mobile Device Management (MDM) schakelt BitLocker bijvoorbeeld automatisch in voor verwisselbare stations, vereist het wachtwoord voor het ontgrendelen van een apparaat en schakelt basisverificatie uit.</span><span class="sxs-lookup"><span data-stu-id="f579d-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="f579d-108">Wanneer een standaardwaarde niet werkt voor uw omgeving, kunt u de basislijn aanpassen om de instellingen toe te passen die u nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="f579d-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f579d-109">Beveiligingslijnlijnen helpen ook bij het instellen van een end-to-end beveiligde werkstroom in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f579d-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f579d-110">Een beveiligingslijn bevat de aanbevolen procedures en aanbevelingen voor instellingen die van invloed zijn op de beveiliging.</span><span class="sxs-lookup"><span data-stu-id="f579d-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f579d-111">Intune werkt samen met het Windows beveiligingsteam dat basislijnen maakt voor groepsbeleid, dus deze aanbevelingen zijn gebaseerd op solide richtlijnen en uitgebreide ervaring.</span><span class="sxs-lookup"><span data-stu-id="f579d-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="f579d-112">Als u in Intune nieuw bent en niet zeker weet waar u moet beginnen, kunt u met beveiligingslijnlijnen snel een beveiligd profiel maken en implementeren.</span><span class="sxs-lookup"><span data-stu-id="f579d-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="f579d-113">Als u momenteel een groepsbeleid gebruikt, is migreren naar Intune voor beheerdoeleinden veel gemakkelijker met beveiligingslijnlijnen, omdat deze zijn ingebouwd in Intune en geavanceerde beheermogelijkheden bevatten.</span><span class="sxs-lookup"><span data-stu-id="f579d-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="f579d-114">Zie voor meer informatie [Windows beveiligingslijnlijnen](/windows/security/threat-protection/windows-security-baselines) en [Mobiel apparaatbeheer.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="f579d-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

