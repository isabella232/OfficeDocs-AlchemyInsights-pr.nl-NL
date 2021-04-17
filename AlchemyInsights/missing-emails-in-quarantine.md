---
title: Ontbrekende e-mailberichten in quarantaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831729"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="831ef-102">Ontbrekende e-mailberichten in quarantaine"</span><span class="sxs-lookup"><span data-stu-id="831ef-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="831ef-103">Beheerders kunnen [deze berichten bekijken,](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide) vrijgeven of verwijderen.</span><span class="sxs-lookup"><span data-stu-id="831ef-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="831ef-104">Als u het beveiligingscentrum & compliancecentrum wilt openen, gaat u naar [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="831ef-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="831ef-105">Als u de pagina Quarantaine rechtstreeks wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="831ef-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="831ef-106">U kunt zoeken op een van de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="831ef-106">You can search by the following values:</span></span>  

- <span data-ttu-id="831ef-107">**Bericht-ID**: de wereldwijd unieke identificatie van het bericht.</span><span class="sxs-lookup"><span data-stu-id="831ef-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="831ef-108">Als u een bericht in de lijst selecteert, wordt de waarde  **Bericht-id**  weergegeven in het flyoutvenster  **Details**  dat wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="831ef-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="831ef-109">Beheerders kunnen [berichttracering](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.</span><span class="sxs-lookup"><span data-stu-id="831ef-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="831ef-110">**E-mailadres afzender**: een enkel e-mailadres van een afzender.</span><span class="sxs-lookup"><span data-stu-id="831ef-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="831ef-111">**E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.</span><span class="sxs-lookup"><span data-stu-id="831ef-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="831ef-112">**Onderwerp**: gebruik het volledige onderwerp van het bericht.</span><span class="sxs-lookup"><span data-stu-id="831ef-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="831ef-113">De zoekopdracht is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="831ef-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="831ef-114">Nadat u de zoekcriteria hebt ingevoerd, klikt u op ![ Knop Vernieuwen vernieuwen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **om** de resultaten te filteren.  </span><span class="sxs-lookup"><span data-stu-id="831ef-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="831ef-115">De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine zijn:</span><span class="sxs-lookup"><span data-stu-id="831ef-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="831ef-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="831ef-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="831ef-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="831ef-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="831ef-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="831ef-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="831ef-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Deze cmdlet is alleen voor berichten, niet voor malwarebestanden van ATP voor SharePoint Online, OneDrive voor Bedrijven of Teams.</span><span class="sxs-lookup"><span data-stu-id="831ef-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="831ef-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="831ef-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)