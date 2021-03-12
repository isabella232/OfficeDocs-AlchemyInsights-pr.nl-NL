---
title: Replicaset
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713746"
---
# <a name="replica-set"></a><span data-ttu-id="e0823-102">Replicaset</span><span class="sxs-lookup"><span data-stu-id="e0823-102">Replica set</span></span>

<span data-ttu-id="e0823-103">AADDS wordt ook wel het beheerde domein genoemd.</span><span class="sxs-lookup"><span data-stu-id="e0823-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="e0823-104">Het zijn eigenlijk twee domeincontrollers die door de back-end worden uitgevoerd en onderhouden.</span><span class="sxs-lookup"><span data-stu-id="e0823-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="e0823-105">De twee dc's bevatten één dc-hoofd en één replicatie-DC.</span><span class="sxs-lookup"><span data-stu-id="e0823-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="e0823-106">Back-ups in AADDS (beheerd domein) zijn een geautomatiseerd proces dat wordt beheerd door het Azure-platform.</span><span class="sxs-lookup"><span data-stu-id="e0823-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="e0823-107">In het geval van een probleem met uw beheerde domein, kan Azure-ondersteuning u helpen bij het terugzetten van de back-up.</span><span class="sxs-lookup"><span data-stu-id="e0823-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="e0823-108">U maakt elke replicaset in een virtueel netwerk.</span><span class="sxs-lookup"><span data-stu-id="e0823-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="e0823-109">Elk virtueel netwerk moet worden doorge peerd naar elk ander virtueel netwerk dat de replicaset van een beheerd domein host.</span><span class="sxs-lookup"><span data-stu-id="e0823-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="e0823-110">Met deze configuratie wordt een mesh-netwerktopologie gemaakt die adreslijstreplicatie ondersteunt.</span><span class="sxs-lookup"><span data-stu-id="e0823-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="e0823-111">Een virtueel netwerk kan meerdere replicasets ondersteunen, mits elke replicaset zich in een ander virtueel subnet plaatst.</span><span class="sxs-lookup"><span data-stu-id="e0823-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="e0823-112">Zie Concepten replicasets voor meer informatie over [de replicaset.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="e0823-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
