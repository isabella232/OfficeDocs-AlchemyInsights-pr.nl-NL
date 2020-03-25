---
title: DLP-regel voor creditcardnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932438"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="93e44-102">DLP problemen met creditcardnummers</span><span class="sxs-lookup"><span data-stu-id="93e44-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="93e44-103">**Belangrijk:** veel SharePoint Online- en OneDrive-klanten draaien bedrijfskritieke toepassingen op de service die op de achtergrond wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="93e44-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="93e44-104">Deze omvatten contentmigratie, Data Loss Prevention (DLP) en back-upoplossingen.</span><span class="sxs-lookup"><span data-stu-id="93e44-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="93e44-105">In deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services in externe werkscenario's zeer beschikbaar en betrouwbaar blijven voor uw gebruikers die afhankelijk zijn van de service.</span><span class="sxs-lookup"><span data-stu-id="93e44-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="93e44-106">Ter ondersteuning van deze doelstelling hebben we strengere beperkingslimieten geïmplementeerd voor achtergrondapps (migratie, DLP en back-upoplossingen) tijdens daguren overdag.</span><span class="sxs-lookup"><span data-stu-id="93e44-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="93e44-107">Je zou verwachten dat deze apps zeer beperkte doorvoer zullen bereiken tijdens deze tijden.</span><span class="sxs-lookup"><span data-stu-id="93e44-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="93e44-108">Tijdens avond- en weekenduren voor de regio is de service echter klaar om een aanzienlijk groter aantal aanvragen van achtergrond-apps te verwerken.</span><span class="sxs-lookup"><span data-stu-id="93e44-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="93e44-109">**DLP problemen met creditcardnummers**</span><span class="sxs-lookup"><span data-stu-id="93e44-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="93e44-110">Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **creditcardnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365?</span><span class="sxs-lookup"><span data-stu-id="93e44-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="93e44-111">Zorg er zo voor dat uw inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="93e44-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="93e44-112">Voor een **creditcardbeleid** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:</span><span class="sxs-lookup"><span data-stu-id="93e44-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="93e44-113">**[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cijfers die kunnen worden opgemaakt of niet-geformatteerd (ddddddddddddddd) en moet de Luhn-test doorstaan.</span><span class="sxs-lookup"><span data-stu-id="93e44-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="93e44-114">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zeer complex en robuust patroon dat kaarten van alle grote merken wereldwijd detecteert, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en dinerkaarten.</span><span class="sxs-lookup"><span data-stu-id="93e44-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="93e44-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, de Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="93e44-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="93e44-116">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="93e44-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="93e44-117">De functie Func_credit_card vindt inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="93e44-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="93e44-118">Een van de volgende is waar:</span><span class="sxs-lookup"><span data-stu-id="93e44-118">One of the following is true:</span></span>

  - <span data-ttu-id="93e44-119">Er wordt een zoekwoord uit Keyword_cc_verification gevonden.</span><span class="sxs-lookup"><span data-stu-id="93e44-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="93e44-120">Er wordt een trefwoord uit Keyword_cc_name gevonden</span><span class="sxs-lookup"><span data-stu-id="93e44-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="93e44-121">De functie Func_expiration_date vindt een datum in de juiste datumnotatie.</span><span class="sxs-lookup"><span data-stu-id="93e44-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="93e44-122">De checksum passeert</span><span class="sxs-lookup"><span data-stu-id="93e44-122">The checksum passes</span></span>

    <span data-ttu-id="93e44-123">De volgende steekproef wordt bijvoorbeeld geactiveerd voor een DLP-creditcardnummerbeleid:</span><span class="sxs-lookup"><span data-stu-id="93e44-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="93e44-124">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="93e44-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="93e44-125">Verloopt: 2/2009</span><span class="sxs-lookup"><span data-stu-id="93e44-125">Expires: 2/2009</span></span>

<span data-ttu-id="93e44-126">Zie het volgende gedeelte in dit artikel voor meer informatie over wat er nodig is om een **creditcardnummer** voor uw inhoud te detecteren: [Wat de gevoelige informatietypen zoeken voor creditcardnummer#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="93e44-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="93e44-127">Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="93e44-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  