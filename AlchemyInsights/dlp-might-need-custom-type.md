---
title: DLP heeft mogelijk een aangepast type nodig
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932653"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8de3a-102">DLP heeft mogelijk een aangepast type nodig</span><span class="sxs-lookup"><span data-stu-id="8de3a-102">DLP might need a custom type</span></span>

<span data-ttu-id="8de3a-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="8de3a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8de3a-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="8de3a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8de3a-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="8de3a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8de3a-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="8de3a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8de3a-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="8de3a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8de3a-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="8de3a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8de3a-109">**DLP vereist mogelijk een aangepast informatietype**</span><span class="sxs-lookup"><span data-stu-id="8de3a-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="8de3a-110">Met een DLP-beleid (Data Loss Prevention) u gevoelige gegevens in uw organisatie identificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="8de3a-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8de3a-111">In sommige scenario's moet u mogelijk uw eigen **aangepaste** gevoelige informatietype maken om de gegevens van uw organisatie te beschermen.</span><span class="sxs-lookup"><span data-stu-id="8de3a-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8de3a-112">Uw organisatie moet bijvoorbeeld werknemers-id's of andere gegevens identificeren en beveiligen in een specifieke indeling voor uw organisatie. Zie in dat dan de volgende artikelen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8de3a-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8de3a-113">**Een ingebouwd gevoelig informatietype aanpassen**</span><span class="sxs-lookup"><span data-stu-id="8de3a-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8de3a-114">Als een ingebouwd gevoelig informatietype met slechts een paar aanpassingen aan uw behoeften zou voldoen, u [een ingebouwd gevoelig informatietype aanpassen.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="8de3a-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8de3a-115">U bijvoorbeeld zoekwoorden toevoegen of verwijderen of ondersteunend bewijsmateriaal toevoegen of verwijderen, zoals een datum of adres.</span><span class="sxs-lookup"><span data-stu-id="8de3a-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8de3a-116">**Een aangepast gevoelig informatietype maken**</span><span class="sxs-lookup"><span data-stu-id="8de3a-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8de3a-117">Maar als u een ander type gevoelige informatie helemaal moet identificeren en beschermen, u [een aangepast gevoelig informatietype maken](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in de gebruikersinterface van het Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="8de3a-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8de3a-118">**Een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8de3a-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8de3a-119">Als de gebruikersinterface ten slotte niet alle opties biedt die u nodig hebt, u [een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="8de3a-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8de3a-120">Door te beginnen met een XML-bestand, u elke beschikbare optie gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8de3a-120">By starting with an XML file, you can use every option available.</span></span>
