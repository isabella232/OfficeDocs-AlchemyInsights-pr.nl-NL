---
title: Problemen met machtigingen tijdens de migratie
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054409"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="27384-102">Gebruikersprofiel en fotosynchronisatie</span><span class="sxs-lookup"><span data-stu-id="27384-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="27384-103">**Profielfoto synchronisatie** -gebruikers kunnen merken dat hun profielfoto niet wordt gesynchroniseerd met SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27384-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="27384-104">Of ze hebben geprobeerd hun profielfoto bij te werken en de foto wordt nog steeds weergegeven als de oude foto.</span><span class="sxs-lookup"><span data-stu-id="27384-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="27384-105">Om ervoor te zorgen dat de profielfoto wordt weergegeven zoals verwacht, moet de gebruiker een fotosynchronisatie starten.</span><span class="sxs-lookup"><span data-stu-id="27384-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="27384-106">Zie [informatie over synchronisatie van profielfoto's in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634) voor meer informatie over het proces voor het synchroniseren van foto's.</span><span class="sxs-lookup"><span data-stu-id="27384-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="27384-107">**Profielsynchronisatie** -de tijd die vereist is voor het voltooien van een profielsynchronisatie is afhankelijk van het aantal wijzigingen (werk) de AD-import taak heeft te verwerken.</span><span class="sxs-lookup"><span data-stu-id="27384-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="27384-108">Als er veel wijzigingen zijn, heeft de timeropdracht veel werk te doen en duurt het langer voordat de wijzigingen worden doorgevoerd in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="27384-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="27384-109">Als de timeropdracht een klein werkvolume heeft, worden de wijzigingen veel sneller doorgevoerd in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="27384-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="27384-110">Zie voor meer informatie over het profielsynchronisatie proces [informatie over synchronisatie van gebruikersprofielen in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="27384-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="27384-111">**Profiel bijwerken in Office duik** -duik gebruikers kunnen hun Office 365-profiel beheren.</span><span class="sxs-lookup"><span data-stu-id="27384-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="27384-112">Zie voor meer informatie, [weergeven en bijwerken van uw profiel in Office duiken](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="27384-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

