---
title: De prestaties van OneDrive oplossen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757880"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="6528e-102">De prestaties van OneDrive oplossen</span><span class="sxs-lookup"><span data-stu-id="6528e-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="6528e-103">Als u een langzamere synchronisatie ondervindt dan verwacht, of vergelijkbare prestatieproblemen met OneDrive:</span><span class="sxs-lookup"><span data-stu-id="6528e-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="6528e-104">Ga na of er geen bekende problemen zijn met het [Dashboard voor de service status](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6528e-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="6528e-105">U kunt [bestanden op aanvraag inschakelen](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , zodat u toegang hebt tot al uw bestanden in OneDrive zonder deze te hoeven downloaden en zonder gebruik te hoeven maken van opslagruimte op uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="6528e-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="6528e-106">[Bekijk aanbevolen procedures](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) voor de netwerk planning en prestaties.</span><span class="sxs-lookup"><span data-stu-id="6528e-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="6528e-107">[Minimaliseer de upload-en downloadsnelheid](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), met name als u een apparaat voor de eerste keer gaat synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="6528e-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="6528e-108">Als u een bibliotheek met meer dan 100.000 items synchroniseert, kan het synchroniseren van OneDrive lang lang lang duren, of de status geeft de verwerking van de 0KB van xMB weer.</span><span class="sxs-lookup"><span data-stu-id="6528e-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="6528e-109">Meer [informatie over het synchroniseren van meer dan 100.000 bestanden](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) en [de ondersteunde limiet 300.000 van OneDrive-bestanden](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="6528e-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="6528e-110">Wanneer een gebruiker de gebruikslimiet overschrijdt, vertraagt SharePoint Online alle verzoeken van die gebruikersaccount gedurende een korte periode.</span><span class="sxs-lookup"><span data-stu-id="6528e-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="6528e-111">Alle gebruikersacties worden vertraagd terwijl de gashendel van kracht is.</span><span class="sxs-lookup"><span data-stu-id="6528e-111">All user actions are throttled while the throttle is in effect.</span></span>
