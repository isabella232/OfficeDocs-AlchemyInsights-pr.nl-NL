---
title: E-mailprofielen gebruiken met Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554979"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="4e635-102">E-mailprofielen gebruiken met Intune</span><span class="sxs-lookup"><span data-stu-id="4e635-102">Using email profiles with Intune</span></span>

<span data-ttu-id="4e635-103">Intune kan worden gebruikt voor het maken en implementeren van e-mailprofielen voor de native (ingebouwde) e-mailclient op meerdere apparaatplatforms.</span><span class="sxs-lookup"><span data-stu-id="4e635-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="4e635-104">[Zie E-mailinstellingen toevoegen aan apparaten met Intune voor](https://docs.microsoft.com/intune/email-settings-configure)informatie over enkele beperkingen die zijn gekoppeld aan e-mailprofielen, waaronder de manier waarop de aanwezigheid van bestaande profielen wordt behandeld en hoe u e-mailprofielen verwijdert.</span><span class="sxs-lookup"><span data-stu-id="4e635-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="4e635-105">Zie voor meer informatie over het maken van e-mailprofielen voor elk apparaatplatform:</span><span class="sxs-lookup"><span data-stu-id="4e635-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="4e635-106">Instellingen voor Android-apparaten voor het configureren van e-mail, verificatie en synchronisatie in Intune</span><span class="sxs-lookup"><span data-stu-id="4e635-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="4e635-107">E-mailinstellingen voor iOS- en iPadOS-apparaten toevoegen in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e635-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="4e635-108">Instellingen voor e-mailprofiel in Microsoft Intune voor apparaten met Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="4e635-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="4e635-109">Instellingen voor e-mailprofiel voor apparaten met Windows 10 in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e635-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="4e635-110">**Veelvoorkomend synchronisatieprobleem**</span><span class="sxs-lookup"><span data-stu-id="4e635-110">**Common syncing issue**</span></span>

<span data-ttu-id="4e635-111">**Een KNOX-e-mailprofiel op Android voorkomt dat gebruikerscontacten, agenda en taken worden gesynchroniseerd met gebruikersapparaten.**</span><span class="sxs-lookup"><span data-stu-id="4e635-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="4e635-112">Het KNOX-e-mailprofiel op Android KNOX biedt de beheerder de mogelijkheid om te bepalen welke inhoudstypen worden gesynchroniseerd met het apparaat door elk op ingeschakeld in te stellen.</span><span class="sxs-lookup"><span data-stu-id="4e635-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="4e635-113">Als de instelling voor een van de inhoudstypen is ingesteld op **Niet geconfigureerd** (het standaard), wordt dat inhoudstype niet automatisch gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="4e635-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="4e635-114">Een gebruiker kan het gewenste inhoudstype rechtstreeks op het apparaat inschakelen, maar die configuratie wordt overschreven door de instelling Intune-beleid en de synchronisatie stopt voor dat inhoudstype.</span><span class="sxs-lookup"><span data-stu-id="4e635-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

