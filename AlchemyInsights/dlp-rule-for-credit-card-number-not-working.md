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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977193"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="46320-102">DLP problemen met creditcardnummers</span><span class="sxs-lookup"><span data-stu-id="46320-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="46320-103">**Belangrijk:** Tijdens deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services zeer beschikbaar blijven - Ga naar [tijdelijke functieaanpassingen van SharePoint Online](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="46320-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="46320-104">**DLP problemen met creditcardnummers**</span><span class="sxs-lookup"><span data-stu-id="46320-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="46320-105">Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **creditcardnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365?</span><span class="sxs-lookup"><span data-stu-id="46320-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="46320-106">Zorg er zo voor dat uw inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="46320-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="46320-107">Voor een **creditcardbeleid** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:</span><span class="sxs-lookup"><span data-stu-id="46320-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="46320-108">**[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cijfers die kunnen worden opgemaakt of niet-geformatteerd (ddddddddddddddd) en moet de Luhn-test doorstaan.</span><span class="sxs-lookup"><span data-stu-id="46320-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="46320-109">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zeer complex en robuust patroon dat kaarten van alle grote merken wereldwijd detecteert, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en dinerkaarten.</span><span class="sxs-lookup"><span data-stu-id="46320-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="46320-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, de Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="46320-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="46320-111">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="46320-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="46320-112">De functie Func_credit_card vindt inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="46320-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="46320-113">Een van de volgende is waar:</span><span class="sxs-lookup"><span data-stu-id="46320-113">One of the following is true:</span></span>

  - <span data-ttu-id="46320-114">Er wordt een zoekwoord uit Keyword_cc_verification gevonden.</span><span class="sxs-lookup"><span data-stu-id="46320-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="46320-115">Er wordt een trefwoord uit Keyword_cc_name gevonden</span><span class="sxs-lookup"><span data-stu-id="46320-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="46320-116">De functie Func_expiration_date vindt een datum in de juiste datumnotatie.</span><span class="sxs-lookup"><span data-stu-id="46320-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="46320-117">De checksum passeert</span><span class="sxs-lookup"><span data-stu-id="46320-117">The checksum passes</span></span>

    <span data-ttu-id="46320-118">De volgende steekproef wordt bijvoorbeeld geactiveerd voor een DLP-creditcardnummerbeleid:</span><span class="sxs-lookup"><span data-stu-id="46320-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="46320-119">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="46320-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="46320-120">Verloopt: 2/2009</span><span class="sxs-lookup"><span data-stu-id="46320-120">Expires: 2/2009</span></span>

<span data-ttu-id="46320-121">Zie het volgende gedeelte in dit artikel voor meer informatie over wat er nodig is om een **creditcardnummer** voor uw inhoud te detecteren: [Wat de gevoelige informatietypen zoeken voor creditcardnummer#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="46320-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="46320-122">Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="46320-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  