---
title: 'AIP: Beleid dat zich niet gedraagt zoals verwacht'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506553"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="6036f-102">AIP: Beleid dat zich niet gedraagt zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="6036f-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="6036f-103">Azure Information Protection: Beleid dat zich niet gedraagt zoals verwacht, zie de volgende richtlijnen voor verschillende beleidsproblemen:</span><span class="sxs-lookup"><span data-stu-id="6036f-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="6036f-104">Als u problemen ondervindt met visuele markeringen, controleert u [Wanneer visuele markeringen worden toegepast.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="6036f-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="6036f-105">Als u problemen ondervindt met automatische etikettering, raadpleegt u [Hoe u de voorwaarden voor automatische en aanbevolen classificatie voor Azure Information Protection configureert](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) en waar de gevoelige [informatietypen naar zoeken.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="6036f-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="6036f-106">Als u problemen ondervindt met native/pfile-beveiliging, raadpleegt u [de configuratie van bestands-API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="6036f-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="6036f-107">Controleer of u scoped policies gebruikt die niet goed zijn geconfigureerd: [het azure-beleid voor informatiebescherming configureren voor specifieke gebruikers met behulp van scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="6036f-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="6036f-108">Als automatische etikettering niet werkt voor Outlook bij het koppelen van een gelabeld document, controleert u of DRMEncryptProperty niet is gedefinieerd zoals hier beschreven: [IRM-registerinstellingen voor beveiliging](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="6036f-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="6036f-109">Als u nog steeds problemen ondervindt, u azure information protection-clientlogboeken verzamelen en de geëxporteerde logboeken aan dit ticket koppelen.</span><span class="sxs-lookup"><span data-stu-id="6036f-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="6036f-110">Open een Office-document of maak een nieuwe e-mail in Outlook.</span><span class="sxs-lookup"><span data-stu-id="6036f-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="6036f-111">Klik op Help en feedback **over bescherming/gevoeligheid**  >  **Help and feedback**.</span><span class="sxs-lookup"><span data-stu-id="6036f-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="6036f-112">Klik **op Logboeken exporteren**.</span><span class="sxs-lookup"><span data-stu-id="6036f-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="6036f-113">Sla de logboeken op naar keuze van de locatie en voeg ze toe aan deze serviceaanvraag.</span><span class="sxs-lookup"><span data-stu-id="6036f-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="6036f-114">Aanvullende informatiebronnen:</span><span class="sxs-lookup"><span data-stu-id="6036f-114">Additional resources:</span></span>

- [<span data-ttu-id="6036f-115">Een label configureren voor visuele markeringen voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6036f-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="6036f-116">Documentatie over Azure Information Protection controleren</span><span class="sxs-lookup"><span data-stu-id="6036f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="6036f-117">Gevoeligheidslabels gebruiken in Office-apps</span><span class="sxs-lookup"><span data-stu-id="6036f-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

