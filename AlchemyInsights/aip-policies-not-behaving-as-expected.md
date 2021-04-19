---
title: 'AIP: Beleidsregels gedragen zich niet zoals verwacht'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821622"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="91ca5-102">AIP: Beleidsregels gedragen zich niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="91ca5-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="91ca5-103">Azure Information Protection: Beleidsregels werken niet zoals verwacht, zie het volgende voor aanbevolen richtlijnen voor verschillende beleidskwesties:</span><span class="sxs-lookup"><span data-stu-id="91ca5-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="91ca5-104">Als u problemen hebt met visuele markeringen, raadpleegt u [Wanneer visuele markeringen worden toegepast.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="91ca5-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="91ca5-105">Als u problemen hebt met automatische labeling, raadpleegt u Voorwaarden configureren voor automatische en aanbevolen classificatie voor [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en Waar de typen gevoelige informatie naar [zoeken.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="91ca5-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="91ca5-106">Als u problemen hebt met de native/pfile-beveiliging, raadpleegt u [bestands-API-configuratie.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="91ca5-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="91ca5-107">Controleer of u beleidsregels met een bereik gebruikt die niet correct zijn geconfigureerd: [Het Azure Information Protection-beleid configureren voor specifieke gebruikers met behulp van beleidsregels met een bereik](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="91ca5-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="91ca5-108">Als automatische labeling niet werkt voor Outlook bij het koppelen van een document met label, controleert u of DRMEncryptProperty niet is gedefinieerd zoals hier wordt beschreven: IRM-registerinstellingen voor [beveiliging.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="91ca5-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="91ca5-109">Als u nog steeds problemen ondervindt, verzamelt u Azure Information Protection-clientlogboeken en koppelt u de geëxporteerde logboeken aan dit ticket.</span><span class="sxs-lookup"><span data-stu-id="91ca5-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="91ca5-110">Open een Office-document of maak een nieuw e-mailbericht in Outlook.</span><span class="sxs-lookup"><span data-stu-id="91ca5-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="91ca5-111">Klik op **Beveiligen/Gevoeligheid** > **Help en feedback**.</span><span class="sxs-lookup"><span data-stu-id="91ca5-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="91ca5-112">Klik op **Logboeken exporteren**.</span><span class="sxs-lookup"><span data-stu-id="91ca5-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="91ca5-113">Sla de logboeken op naar uw keuze van locatie en voeg deze toe aan deze serviceaanvraag.</span><span class="sxs-lookup"><span data-stu-id="91ca5-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="91ca5-114">Aanvullende informatiebronnen:</span><span class="sxs-lookup"><span data-stu-id="91ca5-114">Additional resources:</span></span>

- [<span data-ttu-id="91ca5-115">Een label configureren voor visuele markeringen voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="91ca5-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="91ca5-116">Azure Information Protection-documentatie bekijken</span><span class="sxs-lookup"><span data-stu-id="91ca5-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="91ca5-117">Gevoeligheidslabels gebruiken in Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="91ca5-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

