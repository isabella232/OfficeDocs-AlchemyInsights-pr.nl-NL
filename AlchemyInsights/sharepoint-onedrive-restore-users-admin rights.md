---
title: Problemen met toegang geweigerd berichten naar OneDrive voor bedrijven-sites
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766706"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="c26ea-102">Problemen met toegang geweigerd berichten naar OneDrive voor bedrijven-sites</span><span class="sxs-lookup"><span data-stu-id="c26ea-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="c26ea-103">Dit probleem treedt meestal op wanneer een gebruiker wordt verwijderd en opnieuw gemaakt met de dezelfde UPN (User Principal Name).</span><span class="sxs-lookup"><span data-stu-id="c26ea-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c26ea-104">De nieuwe account wordt gemaakt met behulp van een andere waarde van de PUID (paspoort unieke ID).</span><span class="sxs-lookup"><span data-stu-id="c26ea-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c26ea-105">Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="c26ea-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c26ea-106">Een tweede scenario heeft betrekking op adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OE).</span><span class="sxs-lookup"><span data-stu-id="c26ea-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c26ea-107">Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kunnen dit probleem optreden.</span><span class="sxs-lookup"><span data-stu-id="c26ea-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="c26ea-108">Om dit probleem op te lossen moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [een gebruiker herstellen in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c26ea-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="c26ea-109">Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker uit de OneDrive-site verwijderen met behulp van deze stappen, [een gebruiker verwijderen uit de lijst met gebruikersgegevens]().</span><span class="sxs-lookup"><span data-stu-id="c26ea-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="c26ea-110">Nadat dit is gebeurd, u controleren of de gebruiker beheerdersrechten heeft op de OneDrive-site door de stappen [voor het toevoegen van beheerders voor de onedrive van een gebruiker toe te voegen](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="c26ea-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="c26ea-111">Zie voor meer informatie over machtigingsniveaus het artikel [machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="c26ea-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
