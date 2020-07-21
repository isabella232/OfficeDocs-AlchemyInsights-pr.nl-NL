---
title: Conflicten met SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197936"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="bd6af-102">Conflicten met SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bd6af-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="bd6af-103">Als u fouten ontvangt tijdens een synchronisatie, zoals 'Er bestaat een gesynchroniseerd object met hetzelfde ProxyAddress of UserPrincipalName in uw map', [raadpleegt u Synchronisatiefouten diagnosticeren en herstellen.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)</span><span class="sxs-lookup"><span data-stu-id="bd6af-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="bd6af-104">Overweeg ook dubbele kenmerkbestendigheid in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="bd6af-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="bd6af-105">Zie [Tolerantie voor identiteitssynchronisatie en dubbele kenmerken voor](https://aka.ms/duplicateattributeresiliency)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="bd6af-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>