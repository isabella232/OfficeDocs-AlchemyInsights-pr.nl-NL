---
title: Klassieke SharePoint-auditlogboek rapporten
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662203"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f0b50-102">Auditlogboeken van SharePoint en OneDrive</span><span class="sxs-lookup"><span data-stu-id="f0b50-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f0b50-103">Klassieke SharePoint-controlelogboeken</span><span class="sxs-lookup"><span data-stu-id="f0b50-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f0b50-104">SPO oudere controle is gemigreerd naar een uniform audit logboek (UAL).</span><span class="sxs-lookup"><span data-stu-id="f0b50-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f0b50-105">Alle oudere controlerapporten van SPO worden nu via UAL geactiveerd en de oudere controle signalen zijn gemigreerd naar UAL.</span><span class="sxs-lookup"><span data-stu-id="f0b50-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f0b50-106">Gewijzigde sleutels:</span><span class="sxs-lookup"><span data-stu-id="f0b50-106">Key changes:</span></span>

* <span data-ttu-id="f0b50-107">Bijsnijden is niet beschikbaar als mogelijkheid.</span><span class="sxs-lookup"><span data-stu-id="f0b50-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f0b50-108">Het kiezen van bepaalde gebeurtenissen is niet mogelijk.</span><span class="sxs-lookup"><span data-stu-id="f0b50-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f0b50-109">Raadpleeg [dit document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) voor een volledige lijst met gecontroleerde gebeurtenissen die standaard beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="f0b50-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f0b50-110">De optie **locatie** onder **aangepaste rapporten** is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="f0b50-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f0b50-111">De optie **documenten openen of downloaden** is niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="f0b50-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f0b50-112">Controle-instellingen voor een siteverzameling configureren</span><span class="sxs-lookup"><span data-stu-id="f0b50-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f0b50-113">Modern Unified audit logboeken van SharePoint en OneDrive van compliance</span><span class="sxs-lookup"><span data-stu-id="f0b50-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f0b50-114">Logboekregistratie in Unified audit inschakelen</span><span class="sxs-lookup"><span data-stu-id="f0b50-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f0b50-115">In SharePoint of OneDrive is geen extra configuratie vereist.</span><span class="sxs-lookup"><span data-stu-id="f0b50-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f0b50-116">Gebruik controlelogboekregistratie om de activiteiten van een of meer bestanden, mappen, mappen, gebruikers (s), machtigingen te controleren:</span><span class="sxs-lookup"><span data-stu-id="f0b50-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f0b50-117">Activiteiten van bestanden en pagina's</span><span class="sxs-lookup"><span data-stu-id="f0b50-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f0b50-118">Activiteiten van mappen</span><span class="sxs-lookup"><span data-stu-id="f0b50-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f0b50-119">Activiteiten voordelen en toegang aanvragen</span><span class="sxs-lookup"><span data-stu-id="f0b50-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f0b50-120">Synchronisatieactiviteiten</span><span class="sxs-lookup"><span data-stu-id="f0b50-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f0b50-121">Activiteiten in verband met site beheer</span><span class="sxs-lookup"><span data-stu-id="f0b50-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f0b50-122">Zie in [het auditlogboek zoeken](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)voor meer informatie over het ophalen van deze gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="f0b50-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
