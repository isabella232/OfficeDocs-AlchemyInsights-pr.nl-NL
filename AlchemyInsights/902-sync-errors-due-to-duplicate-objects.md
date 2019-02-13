---
title: 902 (synchronisatiefouten als gevolg van dubbele objecten)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919867"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="849df-102">Synchronisatiefouten als gevolg van dubbele objecten</span><span class="sxs-lookup"><span data-stu-id="849df-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="849df-103">Mogelijk wordt een van de volgende foutberichten weergegeven wanneer adreslijstsynchronisatie is voltooid:</span><span class="sxs-lookup"><span data-stu-id="849df-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="849df-104">Kan dit object in Microsoft Online Services niet bijwerken omdat de volgende kenmerken die zijn gekoppeld aan dit object zijn waarden die al gekoppeld aan een ander object in uw lokale map zijn.</span><span class="sxs-lookup"><span data-stu-id="849df-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="849df-105">Een gesynchroniseerde-object met dezelfde proxyadres bestaat al in de map Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="849df-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="849df-106">Kan dit object niet bijwerken omdat de volgende kenmerken die zijn gekoppeld aan dit object al gekoppeld aan een ander object in uw lokale Active Directory zijn kunnen waarden hebben: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="849df-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="849df-107">Identificeren en oplossen van het probleem, downloaden en uitvoeren van het [IdFix DirSync fout herstel Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="849df-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="849df-108">Zie [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="849df-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

