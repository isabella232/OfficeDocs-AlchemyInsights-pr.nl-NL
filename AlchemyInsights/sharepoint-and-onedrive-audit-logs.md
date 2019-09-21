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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068018"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="a777a-102">Auditlogboeken van SharePoint en OneDrive</span><span class="sxs-lookup"><span data-stu-id="a777a-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="a777a-103">**SharePoint en OneDrive moderne uniforme audit logs van compliance**</span><span class="sxs-lookup"><span data-stu-id="a777a-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="a777a-104">Schakel registratie van Unified audit in/uit</span><span class="sxs-lookup"><span data-stu-id="a777a-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="a777a-105">Er is geen aanvullende configuratie vereist in SharePoint of OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a777a-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="a777a-106">Gebruik controlelogboekregistratie zoeken om te controleren van de activiteit van de bestanden, map (s), gebruiker (s), machtigingen:</span><span class="sxs-lookup"><span data-stu-id="a777a-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="a777a-107">Bestands-en pagina-activiteiten</span><span class="sxs-lookup"><span data-stu-id="a777a-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="a777a-108">Mapactiviteiten</span><span class="sxs-lookup"><span data-stu-id="a777a-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="a777a-109">Activiteiten voordelen en toegang aanvragen</span><span class="sxs-lookup"><span data-stu-id="a777a-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="a777a-110">Synchronisatieactiviteiten</span><span class="sxs-lookup"><span data-stu-id="a777a-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="a777a-111">Activiteiten voor site beheer</span><span class="sxs-lookup"><span data-stu-id="a777a-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="a777a-112">Zie [het controlelogboek doorzoeken](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="a777a-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="a777a-113">**Klassieke SharePoint-audit logboeken**</span><span class="sxs-lookup"><span data-stu-id="a777a-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="a777a-114">We migreerden SPO legacy auditing naar Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="a777a-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="a777a-115">Dit betekent in wezen dat alle SPO verouderde auditverslagen nu worden gevoed via UAL, en de verouderde controle signalen zijn gemigreerd naar UAL.</span><span class="sxs-lookup"><span data-stu-id="a777a-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="a777a-116">Belangrijke wijzigingen:</span><span class="sxs-lookup"><span data-stu-id="a777a-116">Key changes:</span></span>

- <span data-ttu-id="a777a-117">Trimmen als een mogelijkheid is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="a777a-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="a777a-118">De sectie waarin u specifieke gebeurtenissen voor controle kiest, is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="a777a-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="a777a-119">Raadpleeg [dit document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="a777a-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="a777a-120">De optie ' locatie ' onder **aangepaste rapporten** is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="a777a-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="a777a-121">"Openen of downloaden van documenten" gebeurtenissen is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="a777a-121">“Opening or downloading documents” events is NOT available.</span></span> 

