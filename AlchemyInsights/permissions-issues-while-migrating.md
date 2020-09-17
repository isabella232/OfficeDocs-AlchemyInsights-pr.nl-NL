---
title: Problemen met machtigingen tijdens het migreren
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798047"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="84cc2-102">Gebruikersprofiel en foto synchronisatie</span><span class="sxs-lookup"><span data-stu-id="84cc2-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="84cc2-103">**Profielfoto synchronisatie** : gebruikers merken mogelijk dat hun profielfoto niet wordt gesynchroniseerd met SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84cc2-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="84cc2-104">Of de persoon heeft mogelijk geprobeerd hun profielfoto bij te werken en de foto wordt weergegeven als de oude foto.</span><span class="sxs-lookup"><span data-stu-id="84cc2-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="84cc2-105">Om ervoor te zorgen dat de profielfoto wordt weergegeven zoals verwacht, moet de gebruiker een foto synchronisatie starten.</span><span class="sxs-lookup"><span data-stu-id="84cc2-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="84cc2-106">Zie voor meer informatie over het proces van foto synchronisatie [informatie over het synchroniseren van profielafbeeldingen in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="84cc2-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="84cc2-107">**Profielsynchronisatie** -de tijd die nodig is voor het voltooien van een profielsynchronisatie, is afhankelijk van het aantal wijzigingen (werk) dat de AD-import taak moet verwerken.</span><span class="sxs-lookup"><span data-stu-id="84cc2-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="84cc2-108">Als er veel wijzigingen zijn, kan de timertaak veel werk doen en duurt het langer voordat de wijzigingen zijn doorgevoerd in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="84cc2-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="84cc2-109">Als de timeropdracht een klein deel van de hoeveelheid werk bevat, worden de wijzigingen veel sneller doorgevoerd in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="84cc2-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="84cc2-110">Zie [informatie over het synchroniseren van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639) voor meer informatie over het proces van het synchroniseren van profielen.</span><span class="sxs-lookup"><span data-stu-id="84cc2-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="84cc2-111">**Profiel bijwerken in Office Delve** -Delve gebruikers kunnen hun microsoft 365-profiel beheren.</span><span class="sxs-lookup"><span data-stu-id="84cc2-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="84cc2-112">Zie [uw profiel weergeven en bijwerken in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="84cc2-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

