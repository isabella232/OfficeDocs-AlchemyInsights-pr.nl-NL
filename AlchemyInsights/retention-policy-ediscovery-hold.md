---
title: 2609-retentie-of-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994056"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="eed7e-102">Kan geen items verwijderen in SharePoint Online of OneDrive voor bedrijven</span><span class="sxs-lookup"><span data-stu-id="eed7e-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="eed7e-103">U of uw gebruikers mogelijk niet verwijderen van items in SharePoint Online of OneDrive voor bedrijven omdat een bewaarbeleid, bewaar label of eDiscovery-wachtruimte wordt toegepast op een SharePoint van OneDrive-site of een specifiek item.</span><span class="sxs-lookup"><span data-stu-id="eed7e-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="eed7e-104">Dit omvat het niet kunnen verwijderen van een document, een documentversie, een map, een documentbibliotheek, een lijst, een app, een site of een siteverzameling.</span><span class="sxs-lookup"><span data-stu-id="eed7e-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="eed7e-105">Hier volgen enkele voorbeelden van de foutberichten die u ontvangen als u probeert een item te verwijderen dat wordt bewaard:</span><span class="sxs-lookup"><span data-stu-id="eed7e-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="eed7e-106">"Deze site kan niet worden verwijderd omdat deze is opgenomen in een eDiscovery-opslag of bewaarbeleid"</span><span class="sxs-lookup"><span data-stu-id="eed7e-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="eed7e-107">"Deze site heeft een nalevingsbeleid ingesteld op het blokkeren van verwijdering"</span><span class="sxs-lookup"><span data-stu-id="eed7e-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="eed7e-108">"Een nalevingsbeleid blokkeert momenteel deze site verwijdering"</span><span class="sxs-lookup"><span data-stu-id="eed7e-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="eed7e-109">' Deze siteverzameling kan niet worden verwijderd omdat deze sites bevat die deel uitmaken van een eDiscovery-beleid voor vasthouden of bewaren '</span><span class="sxs-lookup"><span data-stu-id="eed7e-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="eed7e-110">"U moet alle items in deze map verwijderen voordat u de map verwijdert"</span><span class="sxs-lookup"><span data-stu-id="eed7e-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="eed7e-111">' Versies van dit item kunnen niet worden verwijderd omdat het in de Houd-of bewaarbeleid staat '</span><span class="sxs-lookup"><span data-stu-id="eed7e-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="eed7e-112">"Item kan niet worden verwijderd tijdens de Hold"</span><span class="sxs-lookup"><span data-stu-id="eed7e-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="eed7e-113">"Het label dat op dit item wordt toegepast, voorkomt dat het wordt bewerkt of verwijderd"</span><span class="sxs-lookup"><span data-stu-id="eed7e-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="eed7e-114">"Lijst kan niet worden verwijderd tijdens het vasthouden of bewaarbeleid"</span><span class="sxs-lookup"><span data-stu-id="eed7e-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="eed7e-115">"De lijst kan niet worden verwijderd als deze is geblokkeerd of als er een bewaarbeleid wordt toegepast"</span><span class="sxs-lookup"><span data-stu-id="eed7e-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="eed7e-116">Als u items in een van deze scenario's wilt verwijderen, moet het bewaarbeleid, het retentie label of de eDiscovery-opslagruimte worden verwijderd (of moet een site worden uitgesloten van een bewaarbeleid).</span><span class="sxs-lookup"><span data-stu-id="eed7e-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="eed7e-117">U moet de respectieve Hold die dit probleem veroorzaakt uitschakelen of uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="eed7e-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="eed7e-118">Nadat een bewaarbeleid of wachtstand is verwijderd, kan het maximaal 24 uur duren voordat de wijziging van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="eed7e-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="eed7e-119">Zie een van de volgende onderwerpen voor informatie over de verschillende retentie-en Hold-functies die kunnen worden toegepast op SharePoint-sites en OneDrive-accounts.</span><span class="sxs-lookup"><span data-stu-id="eed7e-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="eed7e-120">Overzicht van bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="eed7e-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="eed7e-121">Overzicht van inhoudings etiketten</span><span class="sxs-lookup"><span data-stu-id="eed7e-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="eed7e-122">Bewaarplichten beheren in Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="eed7e-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="eed7e-123">eDiscovery houdt</span><span class="sxs-lookup"><span data-stu-id="eed7e-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="eed7e-124">Beleid voor beëindiging en verwijdering van verouderde sites</span><span class="sxs-lookup"><span data-stu-id="eed7e-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
