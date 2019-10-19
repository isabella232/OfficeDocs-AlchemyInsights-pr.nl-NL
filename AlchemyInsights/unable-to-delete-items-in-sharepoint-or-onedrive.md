---
title: Kan geen items verwijderen in SharePoint of OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748539"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a509c-102">Kan items niet verwijderen</span><span class="sxs-lookup"><span data-stu-id="a509c-102">Unable to delete items</span></span>

<span data-ttu-id="a509c-103">Hebt u problemen met het verwijderen van SharePoint-items?</span><span class="sxs-lookup"><span data-stu-id="a509c-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="a509c-104">Zorg er altijd voor dat u over de [juiste machtigingen](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) beschikt om het item te verwijderen of dat de beheerder van een [siteverzameling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) het item probeert te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="a509c-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="a509c-105">Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) is ingesteld voor het item.</span><span class="sxs-lookup"><span data-stu-id="a509c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="a509c-106">Controleer of het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) naar een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="a509c-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="a509c-107">Ten slotte kunnen beheerders [SharePoint-patronen en-procedures](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevatten waarmee u complexe beheeracties uitvoeren, zoals geforceerd verwijderen van hardnekkige items.</span><span class="sxs-lookup"><span data-stu-id="a509c-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a509c-108">PNP-bestand verwijderen</span><span class="sxs-lookup"><span data-stu-id="a509c-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a509c-109">PNP-map verwijderen</span><span class="sxs-lookup"><span data-stu-id="a509c-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a509c-110">PNP-lijst item verwijderen</span><span class="sxs-lookup"><span data-stu-id="a509c-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a509c-111">PNP-lijst verwijderen</span><span class="sxs-lookup"><span data-stu-id="a509c-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a509c-112">PNP-veld verwijderen (kolom)</span><span class="sxs-lookup"><span data-stu-id="a509c-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)