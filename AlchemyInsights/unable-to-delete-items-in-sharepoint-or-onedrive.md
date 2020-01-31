---
title: Items in SharePoint of OneDrive kan niet worden verwijderd
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571241"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="20dbe-102">Kan items niet verwijderen</span><span class="sxs-lookup"><span data-stu-id="20dbe-102">Unable to delete items</span></span>

<span data-ttu-id="20dbe-103">Bewaarbeleid kan dit veroorzaken, u moet de respectievelijke blokkering uitschakelen of uitsluiten die dit probleem veroorzaakt.</span><span class="sxs-lookup"><span data-stu-id="20dbe-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="20dbe-104">Nadat een bewaarbeleid of -blokkering is verwijderd, kan het tot 24 uur duren voordat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="20dbe-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="20dbe-105">Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) is ingesteld op het item.</span><span class="sxs-lookup"><span data-stu-id="20dbe-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="20dbe-106">De site kan de opslaglimiet hebben overschreden, het [sitequotum](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) hebben verhoogd en het item verwijderen.</span><span class="sxs-lookup"><span data-stu-id="20dbe-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="20dbe-107">Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) naar een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="20dbe-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="20dbe-108">Ten slotte kunnen beheerders [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevat waarmee u complexe beheeracties uitvoeren, zoals het verwijderen van hardnekkige items afdwingen.</span><span class="sxs-lookup"><span data-stu-id="20dbe-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="20dbe-109">PNP-bestand verwijderen</span><span class="sxs-lookup"><span data-stu-id="20dbe-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="20dbe-110">PNP-map verwijderen</span><span class="sxs-lookup"><span data-stu-id="20dbe-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="20dbe-111">PNP-lijstitem verwijderen</span><span class="sxs-lookup"><span data-stu-id="20dbe-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="20dbe-112">PNP-lijst verwijderen</span><span class="sxs-lookup"><span data-stu-id="20dbe-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="20dbe-113">PNP-veld verwijderen (kolom)</span><span class="sxs-lookup"><span data-stu-id="20dbe-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)