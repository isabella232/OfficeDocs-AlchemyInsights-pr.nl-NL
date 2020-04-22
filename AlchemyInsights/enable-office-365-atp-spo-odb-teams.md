---
title: Office 365 ATP inschakelen voor SharePoint, OneDrive en Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703421"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="164ff-102">Office 365 geavanceerde bescherming tegen bedreigingen inschakelen voor SharePoint Online, OneDrive en Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="164ff-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="164ff-103">Ga https://protection.office.com naar en meld je aan.</span><span class="sxs-lookup"><span data-stu-id="164ff-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="164ff-104">Kies Veilige bijlagen **voor** > beleid voor**bedreigingsbeheer\*\*\*\*Policy** > .</span><span class="sxs-lookup"><span data-stu-id="164ff-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="164ff-105">Selecteer **ATP inschakelen voor SharePoint, OneDrive en Microsoft Teams**en klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="164ff-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="164ff-106">(Aanbevolen) Voer als globale beheerder of SharePoint Online-beheerder de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uit met de parameter **DisallowInfectedFileDownload** ingesteld op *true.*</span><span class="sxs-lookup"><span data-stu-id="164ff-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="164ff-107">(Aanbevolen) [Waarschuwingen instellen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor gedetecteerde bestanden.</span><span class="sxs-lookup"><span data-stu-id="164ff-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="164ff-108">ATP scant elk bestand in SharePoint Online, OneDrive of Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="164ff-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="164ff-109">Bestanden worden asynchroon gescand, via een proces dat gebruik maakt van gebeurtenissen op het gebied van delen en gastactiviteiten, samen met slimme heuristiek en bedreigingssignalen om schadelijke bestanden te identificeren.</span><span class="sxs-lookup"><span data-stu-id="164ff-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="164ff-110">Zie [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="164ff-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>