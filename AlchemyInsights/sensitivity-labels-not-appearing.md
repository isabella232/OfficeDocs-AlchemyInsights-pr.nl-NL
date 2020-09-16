---
title: Tekstlabels voor vertrouwelijkheid niet weergegeven
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801179"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="ceb23-102">Tekstlabels voor vertrouwelijkheid niet weergegeven</span><span class="sxs-lookup"><span data-stu-id="ceb23-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="ceb23-103">Met gevoelige labels kunt u uw vertrouwelijke inhoud classificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="ceb23-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="ceb23-104">U kunt ze maken in het nalevings centrum van Microsoft 365, Microsoft 365 Beveiligingscentrum of Microsoft 365 Security & compliance, onder classificatie > voor gevoeligheid-labels.</span><span class="sxs-lookup"><span data-stu-id="ceb23-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="ceb23-105">Zie voor meer informatie over deze functie: [overzicht van palletlabels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="ceb23-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="ceb23-106">Controleer het volgende als u uw gevoeligheids labels hebt geconfigureerd, maar deze niet in de Microsoft 365-apps worden weergegeven:</span><span class="sxs-lookup"><span data-stu-id="ceb23-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="ceb23-107">Ga na of het vertrouwelijkheids label is [gepubliceerd](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) naar de gewenste gebruikers en groepen.</span><span class="sxs-lookup"><span data-stu-id="ceb23-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="ceb23-108">Ga na of de gebruiker een app gebruikt die de vertrouwelijkheids labels ondersteunt-Zie [de palletlabels in uw document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="ceb23-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="ceb23-109">Als u [Azure Information Protection-labels migreert](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), moet u rekening houden met de [onderstaande overwegingen.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)</span><span class="sxs-lookup"><span data-stu-id="ceb23-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="ceb23-110">Ondersteuning voor preventie van gegevensverlies (DLP): momenteel kunnen alleen Bewaar labels als voorwaarde worden gebruikt in DLP-beleid.</span><span class="sxs-lookup"><span data-stu-id="ceb23-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="ceb23-111">Ondersteuning voor vertrouwelijkheids labels in een DLP-beleid is nog niet beschikbaar maar we werken eraan.</span><span class="sxs-lookup"><span data-stu-id="ceb23-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="ceb23-112">Wanneer versleuteling op een gevoeligheids label is ingeschakeld, kunt u kiezen voor:</span><span class="sxs-lookup"><span data-stu-id="ceb23-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="ceb23-113">Nu machtigingen toewijzen</span><span class="sxs-lookup"><span data-stu-id="ceb23-113">Assign permissions now</span></span>
    - <span data-ttu-id="ceb23-114">Gebruikersmachtigingen laten toewijzen</span><span class="sxs-lookup"><span data-stu-id="ceb23-114">Let users assign permissions</span></span>


<span data-ttu-id="ceb23-115">Zie [bekende problemen met gevoeligheid-labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)voor meer informatie over mogelijke problemen.</span><span class="sxs-lookup"><span data-stu-id="ceb23-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>