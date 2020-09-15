---
title: Het oplossen van toegang tot berichten van OneDrive voor bedrijven-sites is geweigerd
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670611"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="ddd9b-102">Het oplossen van toegang tot berichten van OneDrive voor bedrijven-sites is geweigerd</span><span class="sxs-lookup"><span data-stu-id="ddd9b-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="ddd9b-103">Dit probleem treedt vaak op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met de UPN (User Principal Name) van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="ddd9b-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ddd9b-104">Het nieuwe account wordt gemaakt met behulp van een andere PUID-waarde (Passport unieke ID).</span><span class="sxs-lookup"><span data-stu-id="ddd9b-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ddd9b-105">Wanneer de gebruiker een siteverzameling of de OneDrive probeert te openen, heeft de gebruiker een onjuiste PUID.</span><span class="sxs-lookup"><span data-stu-id="ddd9b-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ddd9b-106">Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddd9b-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ddd9b-107">Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kan dit probleem zich voordoen.</span><span class="sxs-lookup"><span data-stu-id="ddd9b-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="ddd9b-108">Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="ddd9b-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="ddd9b-109">Als u de oorspronkelijke gebruiker niet kunt terugzetten, verwijdert u de gebruikers uit de OneDrive-site met deze stappen, [verwijdert u een gebruiker uit de lijst gebruikersinfo]().</span><span class="sxs-lookup"><span data-stu-id="ddd9b-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="ddd9b-110">Wanneer dit is gebeurd, kunt u controleren of de gebruiker beheerdersrechten heeft voor de OneDrive-site door de stappen te volgen voor het [toevoegen van beheerders voor onedrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="ddd9b-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="ddd9b-111">Zie het artikel [over machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)voor meer informatie over machtigingsniveaus.</span><span class="sxs-lookup"><span data-stu-id="ddd9b-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
