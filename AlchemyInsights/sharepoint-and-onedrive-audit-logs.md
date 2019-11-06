---
title: Rapporten van de klassieke SharePoint-auditlogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992613"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="9cccf-102">Auditlogboeken van SharePoint en OneDrive</span><span class="sxs-lookup"><span data-stu-id="9cccf-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="9cccf-103">Klassieke SharePoint-audit logboeken</span><span class="sxs-lookup"><span data-stu-id="9cccf-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="9cccf-104">SPO verouderde controle is gemigreerd naar Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="9cccf-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="9cccf-105">Alle SPO verouderde auditrapporten worden nu gevoed via UAL en de verouderde controle signalen zijn gemigreerd naar UAL.</span><span class="sxs-lookup"><span data-stu-id="9cccf-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="9cccf-106">Belangrijke wijzigingen:</span><span class="sxs-lookup"><span data-stu-id="9cccf-106">Key changes:</span></span>

* <span data-ttu-id="9cccf-107">Trimmen is niet beschikbaar als een mogelijkheid.</span><span class="sxs-lookup"><span data-stu-id="9cccf-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="9cccf-108">Het kiezen van specifieke gebeurtenissen om te controleren is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="9cccf-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="9cccf-109">Raadpleeg [dit document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="9cccf-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="9cccf-110">De optie **locatie** onder **aangepaste rapporten** is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="9cccf-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="9cccf-111">De optie **documenten openen of downloaden** is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="9cccf-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="9cccf-112">Controle-instellingen voor een siteverzameling configureren</span><span class="sxs-lookup"><span data-stu-id="9cccf-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="9cccf-113">SharePoint en OneDrive moderne uniforme audit logs van compliance</span><span class="sxs-lookup"><span data-stu-id="9cccf-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="9cccf-114">Schakel registratie van Unified audit in/uit</span><span class="sxs-lookup"><span data-stu-id="9cccf-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="9cccf-115">Er is geen aanvullende configuratie vereist in SharePoint of OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9cccf-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="9cccf-116">Gebruik controlelogboekregistratie zoeken om te controleren van de activiteit van de bestanden, map (s), gebruiker (s), machtigingen:</span><span class="sxs-lookup"><span data-stu-id="9cccf-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="9cccf-117">Bestands-en pagina-activiteiten</span><span class="sxs-lookup"><span data-stu-id="9cccf-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="9cccf-118">Mapactiviteiten</span><span class="sxs-lookup"><span data-stu-id="9cccf-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="9cccf-119">Activiteiten voordelen en toegang aanvragen</span><span class="sxs-lookup"><span data-stu-id="9cccf-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="9cccf-120">Synchronisatieactiviteiten</span><span class="sxs-lookup"><span data-stu-id="9cccf-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="9cccf-121">Activiteiten voor site beheer</span><span class="sxs-lookup"><span data-stu-id="9cccf-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="9cccf-122">Zie [het controlelogboek doorzoeken](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="9cccf-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
