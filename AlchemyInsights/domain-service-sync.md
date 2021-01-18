---
title: Domein service-synchronisatie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884954"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="86ef7-102">Domein service-synchronisatie</span><span class="sxs-lookup"><span data-stu-id="86ef7-102">Domain service synchronization</span></span>

<span data-ttu-id="86ef7-103">Objecten en referenties in een Azure AD DS-domein (Active Directory Domain Services) van Azure Active Directory Domain Services (Azure AD DS) kunnen lokaal binnen het domein worden gemaakt of worden gesynchroniseerd vanuit een Azure Active Directory (Azure AD)-Tenant.</span><span class="sxs-lookup"><span data-stu-id="86ef7-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="86ef7-104">Wanneer u Azure AD DS voor het eerst implementeert, wordt een automatische synchronisatie van eenrichtingssynchronisatie geconfigureerd en gestart met het repliceren van objecten vanuit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="86ef7-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="86ef7-105">Deze eenrichtingssynchronisatie wordt uitgevoerd op de achtergrond om het Azure AD DS-domein up-to-date te houden met wijzigingen in azure AD.</span><span class="sxs-lookup"><span data-stu-id="86ef7-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="86ef7-106">Er vindt geen synchronisatie plaats van Azure AD DS terug in azure AD.</span><span class="sxs-lookup"><span data-stu-id="86ef7-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="86ef7-107">Zie [Domain Service Synchronization (domein service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)) voor meer informatie over het synchroniseren van Azure Active Directory Domain Services.</span><span class="sxs-lookup"><span data-stu-id="86ef7-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
