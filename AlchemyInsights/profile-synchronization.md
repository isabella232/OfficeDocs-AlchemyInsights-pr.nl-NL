---
title: Profielsynchronisatie
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801764"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="49351-102">Wanneer wordt mijn profiel gewijzigd met de SharePoint-app voor gebruikersprofielen?</span><span class="sxs-lookup"><span data-stu-id="49351-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="49351-103">In SharePoint Online wordt de timeropdracht Active Directory-import gebruikt om gebruikers en groepen te importeren in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="49351-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="49351-104">Wijzigingen in de webversie van SharePoint Online worden gesynchroniseerd met de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="49351-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="49351-105">Deze wijzigingen worden in batches verwerkt.</span><span class="sxs-lookup"><span data-stu-id="49351-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="49351-106">De timeropdracht wordt uitgevoerd totdat de wijzigingen worden gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="49351-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="49351-107">Hoe lang het duurt voordat de taak wordt uitgevoerd, is afhankelijk van het aantal wijzigingen in het proces.</span><span class="sxs-lookup"><span data-stu-id="49351-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="49351-108">Een groot aantal wijzigingen duurt langer.</span><span class="sxs-lookup"><span data-stu-id="49351-108">A large number of changes takes longer.</span></span> <span data-ttu-id="49351-109">De SLA (Service Level Agreement) geeft aan dat een wijziging van een gebruiker in de SharePoint Online-Directory binnen 24 uur wordt doorgevoerd in de Gebruikersprofieltoepassing.</span><span class="sxs-lookup"><span data-stu-id="49351-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="49351-110">Meer informatie over het synchroniseren van gebruikersprofielen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="49351-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

