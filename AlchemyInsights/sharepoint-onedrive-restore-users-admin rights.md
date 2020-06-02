---
title: Problemen met geweigerde berichten openen naar OneDrive voor Bedrijven-sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511179"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="fb050-102">Problemen met geweigerde berichten openen naar OneDrive voor Bedrijven-sites</span><span class="sxs-lookup"><span data-stu-id="fb050-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="fb050-103">Dit probleem treedt het vaakst op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde naam van de gebruiker (UPN).</span><span class="sxs-lookup"><span data-stu-id="fb050-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="fb050-104">Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde.</span><span class="sxs-lookup"><span data-stu-id="fb050-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="fb050-105">Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn/haar OneDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="fb050-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="fb050-106">Een tweede scenario omvat adreslijstsynchronisatie met een Organisatie-eenheid (Active Directory organizational unit).</span><span class="sxs-lookup"><span data-stu-id="fb050-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="fb050-107">Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatie worden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.</span><span class="sxs-lookup"><span data-stu-id="fb050-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="fb050-108">Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="fb050-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="fb050-109">Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker met deze stappen verwijderen van de OneDrive-site, [een gebruiker uit de lijst met gebruikersgegevens verwijderen.]()</span><span class="sxs-lookup"><span data-stu-id="fb050-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="fb050-110">Nadat dit is gedaan, u controleren of de gebruiker beheerdersrechten heeft voor de OneDrive-site door de stappen te volgen naar [Beheerders toevoegen voor de OneDrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="fb050-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="fb050-111">Zie het artikel [Machtigingsniveaus in SharePoint voor](https://docs.microsoft.com/sharepoint/understanding-permission-levels)meer informatie over machtigingsniveaus.</span><span class="sxs-lookup"><span data-stu-id="fb050-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
