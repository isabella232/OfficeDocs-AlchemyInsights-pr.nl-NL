---
title: Problemen met toegang tot berichten geweigerd voor OneDrive voor Business-sites
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232517"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="77925-102">Problemen met toegang tot berichten geweigerd voor OneDrive voor Business-sites</span><span class="sxs-lookup"><span data-stu-id="77925-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="77925-103">Dit probleem treedt meestal op wanneer een gebruiker is verwijderd en opnieuw met de dezelfde UPN (User Principal Name gemaakt).</span><span class="sxs-lookup"><span data-stu-id="77925-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="77925-104">De nieuwe account is gemaakt met behulp van een andere waarde voor de PUID (unieke Passport-ID).</span><span class="sxs-lookup"><span data-stu-id="77925-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="77925-105">Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuist PUID.</span><span class="sxs-lookup"><span data-stu-id="77925-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="77925-106">Een tweede scenario heeft betrekking op directory synchronisatie met een organisatie-eenheid (OU) van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77925-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="77925-107">Als gebruikers hebben al aangemeld bij SharePoint, worden verplaatst naar een andere organisatie-eenheid en resynced met SharePoint, kunnen zij dit probleem optreden.</span><span class="sxs-lookup"><span data-stu-id="77925-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="77925-108">Om dit probleem te verhelpen moet u weer de oorspronkelijke UPN met de stappen in het artikel, het[herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="77925-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="77925-109">Als u de oorspronkelijke gebruiker niet kunt herstellen, moet u de oude gebruiker verwijderen uit de OneDrive-site met behulp van deze stappen [verwijdert u een gebruiker uit de lijst met gebruikersgegevens]().</span><span class="sxs-lookup"><span data-stu-id="77925-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="77925-110">Nadat dit is gebeurd, kunt u controleren of dat de gebruiker heeft admin rechten op de OneDrive website met de volgende stappen om [admin toevoegen voor OneDrive van de gebruiker de](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="77925-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="77925-111">Zie voor meer informatie over machtigingsniveaus, het artikel, [Wat zijn machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="77925-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
