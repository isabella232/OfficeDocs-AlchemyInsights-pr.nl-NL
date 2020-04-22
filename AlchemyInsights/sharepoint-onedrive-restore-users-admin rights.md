---
title: Probleemoplossing Toegang geweigerde berichten naar OneDrive voor Bedrijven-sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692796"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="2d2da-102">Probleemoplossing Toegang geweigerde berichten naar OneDrive voor Bedrijven-sites</span><span class="sxs-lookup"><span data-stu-id="2d2da-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="2d2da-103">Dit probleem treedt het vaakst op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde gebruikersnaam (UPN).</span><span class="sxs-lookup"><span data-stu-id="2d2da-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="2d2da-104">Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde.</span><span class="sxs-lookup"><span data-stu-id="2d2da-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="2d2da-105">Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn OfaDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="2d2da-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="2d2da-106">Een tweede scenario omvat adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OU).</span><span class="sxs-lookup"><span data-stu-id="2d2da-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="2d2da-107">Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatieworden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.</span><span class="sxs-lookup"><span data-stu-id="2d2da-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="2d2da-108">Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="2d2da-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="2d2da-109">Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker met deze stappen van de OneDrive-site verwijderen, [een gebruiker verwijderen uit de lijst met gebruikersgegevens]().</span><span class="sxs-lookup"><span data-stu-id="2d2da-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="2d2da-110">Nadat dit is gebeurd, u controleren of de gebruiker beheerdersrechten heeft op de OneDrive-site door de stappen te volgen om beheerders toe te [voegen voor de OneDrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="2d2da-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="2d2da-111">Zie het artikel [Machtigingsniveaus in SharePoint voor](https://docs.microsoft.com/sharepoint/understanding-permission-levels)meer informatie over machtigingsniveaus.</span><span class="sxs-lookup"><span data-stu-id="2d2da-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
