---
title: Kan niet verwijderen van items in SharePoint of OneDrive
ms.author: kirks
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
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366528"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="8895d-102">Kan geen items verwijderen</span><span class="sxs-lookup"><span data-stu-id="8895d-102">Unable to delete items</span></span>

<span data-ttu-id="8895d-103">Hebt u problemen items verwijderen?</span><span class="sxs-lookup"><span data-stu-id="8895d-103">Having issues deleting items?</span></span>

- <span data-ttu-id="8895d-104">Controleer altijd of u beschikt over de [juiste machtigingen](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) te verwijderen van het item of een poging tot [beheerder van de siteverzameling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) het item verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8895d-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="8895d-105">Zorg ervoor dat er niet een [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) instellen op het item.</span><span class="sxs-lookup"><span data-stu-id="8895d-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="8895d-106">Controleer dat het item niet is [uitgecheckt door](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="8895d-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="8895d-107">Ten slotte kunnen beheerders gebruiken [SharePoint patronen en werkwijzen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) met een bibliotheek met PowerShell-opdrachten waarmee u acties uit te voeren complexe management, zoals force stubborn items verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8895d-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="8895d-108">PNP-bestand verwijderen</span><span class="sxs-lookup"><span data-stu-id="8895d-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="8895d-109">PNP-map verwijderen</span><span class="sxs-lookup"><span data-stu-id="8895d-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="8895d-110">Met PNP-lijstitem verwijderen</span><span class="sxs-lookup"><span data-stu-id="8895d-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="8895d-111">Plug en Play lijst verwijderen</span><span class="sxs-lookup"><span data-stu-id="8895d-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="8895d-112">Verwijderen van PNP-veld (kolom)</span><span class="sxs-lookup"><span data-stu-id="8895d-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)