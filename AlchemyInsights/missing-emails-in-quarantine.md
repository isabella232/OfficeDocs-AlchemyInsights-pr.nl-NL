---
title: Ontbrekende e-mails in quarantaine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569047"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="9fb2f-102">Ontbrekende e-mails in quarantaine"</span><span class="sxs-lookup"><span data-stu-id="9fb2f-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="9fb2f-103">Beheerders kunnen [deze berichten bekijken, vrijgeven of verwijderen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9fb2f-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="9fb2f-104">& Ga naar [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="9fb2f-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="9fb2f-105">Als u de quarantainepagina rechtstreeks wilt openen, gaat u naar [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="9fb2f-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="9fb2f-106">U kunt zoeken op een van de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="9fb2f-106">You can search by the following values:</span></span>  

- <span data-ttu-id="9fb2f-107">**Bericht-ID**: de wereldwijd unieke identificatie van het bericht.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="9fb2f-108">Als u een bericht in de lijst selecteert, wordt de waarde **bericht-id** weergegeven in het flyoutvenster **Details** dat wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="9fb2f-109">Beheerders kunnen [berichttracering](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) gebruiken om naar berichten en de bijbehorende bericht-ID’s te zoeken.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="9fb2f-110">**E-mailadres afzender**: een enkel e-mailadres van een afzender.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="9fb2f-111">**E-mailadres ontvanger**: een enkel e-mailadres van een ontvanger.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="9fb2f-112">**Onderwerp**: gebruik het volledige onderwerp van het bericht.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="9fb2f-113">De zoekopdracht is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="9fb2f-114">Nadat u de zoekcriteria hebt ingevoerd, klikt u op ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Vernieuwen** om de resultaten te filteren.  </span><span class="sxs-lookup"><span data-stu-id="9fb2f-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="9fb2f-115">De cmdlets die u gebruikt om berichten en bestanden in quarantaine te bekijken en te beheren zijn:</span><span class="sxs-lookup"><span data-stu-id="9fb2f-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="9fb2f-116">Bericht in quarantaine verwijderen</span><span class="sxs-lookup"><span data-stu-id="9fb2f-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="9fb2f-117">In quarantaine exporterenMessage</span><span class="sxs-lookup"><span data-stu-id="9fb2f-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="9fb2f-118">In quarantaine plaatsenMessage</span><span class="sxs-lookup"><span data-stu-id="9fb2f-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="9fb2f-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Houd er rekening mee dat deze cmdlet alleen is voor berichten, niet voor malwarebestanden van ATP voor SharePoint Online, OneDrive voor Bedrijven of Teams.</span><span class="sxs-lookup"><span data-stu-id="9fb2f-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="9fb2f-120">Release-quarantineMessage</span><span class="sxs-lookup"><span data-stu-id="9fb2f-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)