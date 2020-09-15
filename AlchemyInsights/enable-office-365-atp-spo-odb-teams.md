---
title: Office 365 ATP inschakelen voor SharePoint, OneDrive en Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709902"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ed1e0-102">Office 365 Advanced Threat Protection inschakelen voor SharePoint Online, OneDrive en Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ed1e0-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ed1e0-103">Ga naar https://protection.office.com en meld u aan.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ed1e0-104">Selecteer **Threat management**  >  **Policy**  >  **veilige bijlagen**voor het beleid voor bedreigings beheer.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ed1e0-105">Selecteer **ATP voor SharePoint, OneDrive en Microsoft teams inschakelen**en klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ed1e0-106">Beter Als globale beheerder of een SharePoint Online-beheerder voert u de cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uit waarbij de **DisallowInfectedFileDownload** -parameter is ingesteld op *waar*.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ed1e0-107">Beter [Waarschuwingen instellen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor gedetecteerde bestanden.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ed1e0-108">Met ATP kan ik elk afzonderlijk bestand in SharePoint Online, OneDrive of Microsoft teams scannen.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ed1e0-109">Bestanden worden asynchroon gescand, via een proces waarbij gebeurtenissen voordelen en gebeurtenissen met gebeurtenissen van een gast worden gebruikt, samen met slimme heuristische en bedreigings signalen om kwaadaardige bestanden te identificeren.</span><span class="sxs-lookup"><span data-stu-id="ed1e0-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ed1e0-110">Bekijk [ATP voor SharePoint, OneDrive en Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ed1e0-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>