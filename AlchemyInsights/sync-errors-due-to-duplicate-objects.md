---
title: 902 (synchronisatiefouten door dubbele objecten)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737336"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d0167-102">Synchronisatiefouten door dubbele objecten</span><span class="sxs-lookup"><span data-stu-id="d0167-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d0167-103">Mogelijk wordt een van de volgende foutberichten weergegeven wanneer adreslijstsynchronisatie is voltooid in Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d0167-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="d0167-104">Kan dit object in Microsoft Online Services niet bijwerken omdat de volgende kenmerken van dit object waarden bevatten die mogelijk al aan een ander object in de lokale adreslijst zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="d0167-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="d0167-105">De Microsoft Online Services-map bestaat al met een gesynchroniseerd object dat hetzelfde proxyadres bevat.</span><span class="sxs-lookup"><span data-stu-id="d0167-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="d0167-106">Kan dit object niet bijwerken omdat de volgende kenmerken die aan dit object zijn gekoppeld waarden bevatten die mogelijk al aan een ander object in de lokale adreslijstservices zijn gekoppeld: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="d0167-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="d0167-107">Als u het probleem wilt identificeren en oplossen, downloadt en voert u het [hulpprogramma IdFix DirSync-foutherstel](https://www.microsoft.com/download/details.aspx?id=36832)uit.</span><span class="sxs-lookup"><span data-stu-id="d0167-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="d0167-108">Zie [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d0167-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
