---
title: Kan geen items verwijderen in SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806106"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="59dfe-102">Items kunnen niet worden verwijderd</span><span class="sxs-lookup"><span data-stu-id="59dfe-102">Unable to delete items</span></span>

<span data-ttu-id="59dfe-103">Het bewaarbeleid kan dit veroorzaken, u dient de juiste bewaring uit te schakelen of te uitsluiten die dit probleem veroorzaakt.</span><span class="sxs-lookup"><span data-stu-id="59dfe-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="59dfe-104">Nadat het bewaarbeleid of de bewaring is verwijderd, duurt het maximaal 24 uur voordat de wijziging is doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="59dfe-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="59dfe-105">Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) is ingesteld voor het item.</span><span class="sxs-lookup"><span data-stu-id="59dfe-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="59dfe-106">De site heeft mogelijk een beperkte opslagruimte, Verhoog de [Sitequota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) en verwijder het item.</span><span class="sxs-lookup"><span data-stu-id="59dfe-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="59dfe-107">Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) door een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="59dfe-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="59dfe-108">Ten slotte kunnen beheerders gebruikmaken van [SharePoint-patronen en-procedures](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) met een bibliotheek met PowerShell-opdrachten waarmee u complexe beheeracties kunt uitvoeren, zoals het verwijderen van stubborn-items.</span><span class="sxs-lookup"><span data-stu-id="59dfe-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="59dfe-109">PNP-bestand verwijderen</span><span class="sxs-lookup"><span data-stu-id="59dfe-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="59dfe-110">PNP-map verwijderen</span><span class="sxs-lookup"><span data-stu-id="59dfe-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="59dfe-111">PNP-lijst item verwijderen</span><span class="sxs-lookup"><span data-stu-id="59dfe-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="59dfe-112">PNP-lijst verwijderen</span><span class="sxs-lookup"><span data-stu-id="59dfe-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="59dfe-113">PNP-veld (kolom) verwijderen</span><span class="sxs-lookup"><span data-stu-id="59dfe-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)