---
title: DLP-beleidstips werken niet
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932581"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="dc97b-102">Problemen met DLP-beleidstip</span><span class="sxs-lookup"><span data-stu-id="dc97b-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="dc97b-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="dc97b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dc97b-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="dc97b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dc97b-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="dc97b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dc97b-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="dc97b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dc97b-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="dc97b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dc97b-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="dc97b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dc97b-109">**DLP-beleidstips**</span><span class="sxs-lookup"><span data-stu-id="dc97b-109">**DLP policy tips**</span></span>

<span data-ttu-id="dc97b-110">Bij het gebruik van **DLP-beleid**kunnen gebruikers op de hoogte worden gesteld van een beleidsschending met **beleidstips**.</span><span class="sxs-lookup"><span data-stu-id="dc97b-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="dc97b-111">Beheerders kunnen beleidstips configureren om weer te geven tijdens het testen van hun DLP-beleid of wanneer het beleid in de volledige handhavingsmodus staat.</span><span class="sxs-lookup"><span data-stu-id="dc97b-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="dc97b-112">Ga als volgt te werk om beleidstips over uw DLP-beleid in het beveiligings- en nalevingscentrum in de volledige handhavingsmodus te configureren:</span><span class="sxs-lookup"><span data-stu-id="dc97b-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="dc97b-113">Controleer of beleidstips zijn **ingeschakeld** op de DLP-regel met behulp van de [stappen hier](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="dc97b-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="dc97b-114">Zorg ervoor dat uw **inhoud overeenkomt met** wat **nodig** is om de regel in dit artikel [hier](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)te activeren.</span><span class="sxs-lookup"><span data-stu-id="dc97b-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="dc97b-115">Beleidstips worden weergegeven in zowel OWA als Outlook.</span><span class="sxs-lookup"><span data-stu-id="dc97b-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="dc97b-116">Wanneer u **Outlook 2013 of hoger**gebruikt, worden beleidstips echter alleen onder bepaalde voorwaarden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="dc97b-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="dc97b-117">Deze voorwaarden worden hier weergegeven: [Ondersteunde voorwaarden voor Outlook 2013 of hoger voor het weergeven van beleidstips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="dc97b-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="dc97b-118">Zie [Beleidstips voor DLP-beleid](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) voor meer informatie over DLP-beleidstips</span><span class="sxs-lookup"><span data-stu-id="dc97b-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  