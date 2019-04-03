---
title: Office 365 ATP inschakelen voor SharePoint en OneDrive Microsoft-Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030934"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="444cf-102">Office 365 bedreiging voor geavanceerde beveiliging voor SharePoint Online, OneDrive en Microsoft-Teams</span><span class="sxs-lookup"><span data-stu-id="444cf-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="444cf-103">Ga naar https://protection.office.com en log in.</span><span class="sxs-lookup"><span data-stu-id="444cf-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="444cf-104">Kies **Threat management** > **beleid** > **Veilige bijlagen**.</span><span class="sxs-lookup"><span data-stu-id="444cf-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="444cf-105">Selecteer **ATP voor SharePoint, OneDrive, en Microsoft-Teams inschakelen**en klik vervolgens op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="444cf-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="444cf-106">(Aanbevolen) Als een globale beheerder of beheerder van een SharePoint Online, de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) worden uitgevoerd met de parameter **DisallowInfectedFileDownload** is ingesteld op *true*.</span><span class="sxs-lookup"><span data-stu-id="444cf-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="444cf-107">(Aanbevolen) [Waarschuwingen instellen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor bestanden gevonden.</span><span class="sxs-lookup"><span data-stu-id="444cf-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="444cf-108">ATP wordt nom scan van elk bestand in SharePoint Online, OneDrive of Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="444cf-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="444cf-109">Bestanden gescand asynchroon, via een proces dat gebruikmaakt van delen en Gast activiteitsgebeurtenissen en intelligente heuristiek en bedreiging signalen om schadelijke bestanden te identificeren.</span><span class="sxs-lookup"><span data-stu-id="444cf-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="444cf-110">Zie [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="444cf-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>