---
title: Informatie over Yammer-beheerders
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035730"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="de761-102">Informatie over Yammer-beheerders</span><span class="sxs-lookup"><span data-stu-id="de761-102">About Yammer admins</span></span>

<span data-ttu-id="de761-103">**Netwerkbeheerders**</span><span class="sxs-lookup"><span data-stu-id="de761-103">**Network admins**</span></span>

<span data-ttu-id="de761-104">Globale beheerders worden automatisch gepromoveerd naar de rol geverifieerde beheerder in een Yammer-netwerk.</span><span class="sxs-lookup"><span data-stu-id="de761-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="de761-105">In de volgende gevallen kan deze promotie niet correct worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="de761-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="de761-106">Er bestaan meerdere Yammer-netwerken en de beheerder wordt aangemeld bij de verkeerde.</span><span class="sxs-lookup"><span data-stu-id="de761-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="de761-107">[Netwerkconsolidatie](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is vereist om één Yammer-netwerk te kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="de761-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="de761-108">Azure PIM wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="de761-108">Azure PIM is being used.</span></span> <span data-ttu-id="de761-109">De gebruiker wordt mogelijk niet lang genoeg gepromoveerd tot globale beheerder om de promotie te kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="de761-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="de761-110">Een toekomstige update voor Yammer kan dit probleem oplossen, maar het is het beste om gebruikers handmatig te promoveren naar globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="de761-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="de761-111">Er is een synchronisatieprobleem met het Yammer-netwerk.</span><span class="sxs-lookup"><span data-stu-id="de761-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="de761-112">In dit geval is een ondersteuningsaanvraag vereist voor verder onderzoek.</span><span class="sxs-lookup"><span data-stu-id="de761-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="de761-113">Zie Yammer-beheerders beheren voor meer informatie over [Yammer-beheerdersrollen.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="de761-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="de761-114">**Groepsbeheerders**</span><span class="sxs-lookup"><span data-stu-id="de761-114">**Group admins**</span></span>

<span data-ttu-id="de761-115">Groepsbeheerders voor verbonden groepen van Microsoft 365 worden gesynchroniseerd met groepslidmaatschap vanuit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de761-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="de761-116">Voor grote groepen kan deze synchronisatie een langere periode duren.</span><span class="sxs-lookup"><span data-stu-id="de761-116">For large groups, this sync can take an extended period.</span></span>
