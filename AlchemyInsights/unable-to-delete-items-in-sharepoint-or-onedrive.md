---
title: Items in SharePoint of OneDrive niet kunnen verwijderen
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511971"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="c9d3a-102">Items niet kunnen verwijderen</span><span class="sxs-lookup"><span data-stu-id="c9d3a-102">Unable to delete items</span></span>

<span data-ttu-id="c9d3a-103">Bewaarbeleid kan dit veroorzaken, u moet de betreffende blokkering die dit probleem veroorzaakt uitschakelen of uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="c9d3a-104">Nadat een bewaarbeleid of blokkering is verwijderd, kan het tot 24 uur duren voordat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="c9d3a-105">Zorg ervoor dat er geen instelling voor [bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) op het item staat.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="c9d3a-106">De site heeft mogelijk de opslaglimiet overschreden, het [sitequotum](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) verhoogd en het item verwijderd.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="c9d3a-107">Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) bij een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="c9d3a-108">Ten slotte kunnen beheerders [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevat waarmee u complexe beheeracties uitvoeren, zoals het forceren van hardnekkige items.</span><span class="sxs-lookup"><span data-stu-id="c9d3a-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="c9d3a-109">PNP-bestand verwijderen</span><span class="sxs-lookup"><span data-stu-id="c9d3a-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="c9d3a-110">PNP-map verwijderen</span><span class="sxs-lookup"><span data-stu-id="c9d3a-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="c9d3a-111">PNP-lijstitem verwijderen</span><span class="sxs-lookup"><span data-stu-id="c9d3a-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="c9d3a-112">PNP-lijst verwijderen</span><span class="sxs-lookup"><span data-stu-id="c9d3a-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="c9d3a-113">PNP-veld verwijderen (kolom)</span><span class="sxs-lookup"><span data-stu-id="c9d3a-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)