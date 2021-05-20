---
title: Schakel Office 365 ATP in voor SharePoint, OneDrive en Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543923"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="7a967-102">Microsoft Defender inschakelen voor Office 365 voor SharePoint Online, OneDrive en Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7a967-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="7a967-103">Ga naar https://protection.office.com en meld u aan.</span><span class="sxs-lookup"><span data-stu-id="7a967-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="7a967-104">Kies **Bedreigingsbeheerbeleid**  >    >  **Safe Bijlagen**.</span><span class="sxs-lookup"><span data-stu-id="7a967-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="7a967-105">Selecteer **Defender in Office 365 voor SharePoint, OneDrive en Microsoft Teams** en klik vervolgens op **Opslaan.**</span><span class="sxs-lookup"><span data-stu-id="7a967-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="7a967-106">(Aanbevolen) Als globale beheerder of SharePoint Online-beheerder kunt u de cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uitvoeren met de parameter **DisallowInfectedFileDownload** die is ingesteld op *true.*</span><span class="sxs-lookup"><span data-stu-id="7a967-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="7a967-107">(Aanbevolen) [Waarschuwingen instellen voor](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) gedetecteerde bestanden.</span><span class="sxs-lookup"><span data-stu-id="7a967-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="7a967-108">Microsoft Defender voor Office 365 scant niet elk bestand in SharePoint Online, OneDrive of Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7a967-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="7a967-109">Bestanden worden asynchroon gescand, via een proces dat gebruikmaakt van gebeurtenissen voor delen en gastactiviteit, samen met slimme heuristische en bedreigingssignalen om schadelijke bestanden te identificeren.</span><span class="sxs-lookup"><span data-stu-id="7a967-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="7a967-110">Zie [Microsoft Defender voor Office 365 voor SharePoint, OneDrive en Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="7a967-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>