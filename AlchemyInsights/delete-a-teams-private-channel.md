---
title: Een privékanaal van Teams verwijderen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438990"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="8e9e9-102">Een privékanaal van Teams verwijderen</span><span class="sxs-lookup"><span data-stu-id="8e9e9-102">Delete a Teams private channel</span></span>

<span data-ttu-id="8e9e9-103">Microsoft is op de hoogte van een probleem met het verwijderen van een privékanaal van Teams als u SharePoint-bewaarbeleid hebt ingeschakeld voor de onderliggende SharePoint-site.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="8e9e9-104">Microsoft werkt aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="8e9e9-105">In de tussentijd u de volgende tijdelijke oplossingen gebruiken om het privékanaal te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="8e9e9-106">**Sluit de team-siteverzameling uit van het retentiebeleid van Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="8e9e9-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="8e9e9-107">Ga naar de Office 365-beheerportal en selecteer **Alles weergeven** in het linkernavigatiedeelvenster.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="8e9e9-108">Ga onder **Beheercentra**naar het beleid voor het voorkomen **van nalevingsgegevensverlies**op het gebied van  >  **&**  >  **nalevingsgegevens.**</span><span class="sxs-lookup"><span data-stu-id="8e9e9-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="8e9e9-109">Identificeer een beleid dat van toepassing is op Sharepoint-sites en wijzig het beleid, zodat de Sharepoint-site voor het team dat het privékanaal bevat, NIET is opgenomen onder het bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="8e9e9-110">Sla het beleid op.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-110">Save the policy.</span></span>
    <span data-ttu-id="8e9e9-111">Het kan tot 24 uur duren voordat beleidsinstellingen van kracht worden.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="8e9e9-112">Nadat de site is uitgesloten, u het privékanaal verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="8e9e9-113">Mogelijk ***kunt*** u het privékanaal verwijderen met Microsoft Teams op uw Android-apparaat.</span><span class="sxs-lookup"><span data-stu-id="8e9e9-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="8e9e9-114">Zie [Niet in staat om items te verwijderen in SharePoint Online of OneDrive voor Bedrijven](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)voor gerelateerde SharePoint-informatie .</span><span class="sxs-lookup"><span data-stu-id="8e9e9-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>