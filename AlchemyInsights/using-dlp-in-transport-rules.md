---
title: DLP gebruiken in transportregels
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915092"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="9d424-102">DLP gebruiken in transportregels</span><span class="sxs-lookup"><span data-stu-id="9d424-102">Using DLP in transport rules</span></span>

<span data-ttu-id="9d424-103">Als u Preventie van gegevensverlies (DLP) wilt integreren in een bestaand transport, gebruikt u de voorwaarde '**Als het bericht...bevat Gevoelige informatie**' in de instelling van de transportregel.</span><span class="sxs-lookup"><span data-stu-id="9d424-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="9d424-104">**Voor meer informatie raadpleegt u:**</span><span class="sxs-lookup"><span data-stu-id="9d424-104">**For more details, see:**</span></span>

- <span data-ttu-id="9d424-105">Geïntegreerde DLP-gevoelige gegevenstypen in transportregels: [Regels voor gevoelige informatie integreren](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="9d424-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="9d424-106">U kunt de regel ook met of zonder beleidstest testen met behulp van de Testmodus van de regel.</span><span class="sxs-lookup"><span data-stu-id="9d424-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="9d424-107">U moet 30 min. wachten na het maken van de regel voordat u deze kunt testen.</span><span class="sxs-lookup"><span data-stu-id="9d424-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="9d424-108">Zie [Testmailstroom/transportregels](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="9d424-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="9d424-109">**Opmerking**: Als u een nieuw DLP-beleid wilt implementeren met transportregels in de SBV, gebruikt u in plaats daarvan [DLP-beleid in het Beveiligings- en Compliancecentrum](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="9d424-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
