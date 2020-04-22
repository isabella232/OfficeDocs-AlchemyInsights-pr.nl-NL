---
title: 902 (Synchronisatiefouten als gevolg van dubbele objecten)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767114"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="50adf-102">Synchronisatiefouten als gevolg van dubbele objecten</span><span class="sxs-lookup"><span data-stu-id="50adf-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="50adf-103">Mogelijk ontvangt u een van de volgende foutmeldingen wanneer de synchronisatie van de map is voltooid in Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="50adf-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="50adf-104">Kan dit object niet bijwerken in Microsoft Online Services omdat de volgende kenmerken die aan dit object zijn gekoppeld, waarden bevatten die mogelijk al zijn gekoppeld aan een ander object in uw lokale map.</span><span class="sxs-lookup"><span data-stu-id="50adf-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="50adf-105">Er bestaat al een gesynchroniseerd object met hetzelfde proxyadres in uw microsoft online services-map.</span><span class="sxs-lookup"><span data-stu-id="50adf-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="50adf-106">Kan dit object niet bijwerken omdat de volgende kenmerken die aan dit object zijn gekoppeld, waarden bevatten die mogelijk al zijn gekoppeld aan een ander object in uw lokale directoryservices: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="50adf-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="50adf-107">Download en voer het Hulpprogramma voor het oplossen van de [Foutherstel van IdFix](https://www.microsoft.com/download/details.aspx?id=36832)uit om het probleem te identificeren en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="50adf-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="50adf-108">Zie [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="50adf-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
