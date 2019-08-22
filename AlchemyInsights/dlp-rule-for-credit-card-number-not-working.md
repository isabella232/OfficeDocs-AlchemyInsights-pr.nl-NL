---
title: DLP-regel voor het nummer van de creditcard niet werkt
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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529950"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="2d1cd-102">Problemen met nummers van creditcards DLP</span><span class="sxs-lookup"><span data-stu-id="2d1cd-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="2d1cd-103">Ondervindt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud met een **Creditcardnummer** als u een type DLP gevoelige informatie in O365?</span><span class="sxs-lookup"><span data-stu-id="2d1cd-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2d1cd-104">Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor het starten van de het DLP-beleid als het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="2d1cd-105">Bijvoorbeeld voor een **creditcard beleid** geconfigureerd met een betrouwbaarheidsniveau van 85%, het volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren:</span><span class="sxs-lookup"><span data-stu-id="2d1cd-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2d1cd-106">**[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cijfers nauwkeurig, hetgeen kunnen worden opgemaakt of niet-opgemaakte (dddddddddddddddd) en de test Luhn moet doorgeven.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="2d1cd-107">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Krachtige en zeer complex patroon dat kaarten van alle belangrijke merken over de hele wereld, met inbegrip van Visa, MasterCard, Discover Card, JCB, American Express, cadeaubonnen en diner kaarten detecteert.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="2d1cd-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, de controlesom Luhn</span><span class="sxs-lookup"><span data-stu-id="2d1cd-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="2d1cd-109">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Een DLP-beleid is 85% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="2d1cd-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2d1cd-110">De functie Func_credit_card wordt gezocht naar inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2d1cd-111">Het volgende geldt:</span><span class="sxs-lookup"><span data-stu-id="2d1cd-111">One of the following is true:</span></span>

  - <span data-ttu-id="2d1cd-112">Een sleutelwoord Keyword_cc_verification is gevonden.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="2d1cd-113">Een sleutelwoord Keyword_cc_name is gevonden.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="2d1cd-114">De functie Func_expiration_date wordt een datum in de juiste notatie.</span><span class="sxs-lookup"><span data-stu-id="2d1cd-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="2d1cd-115">De controlesom wordt doorgegeven</span><span class="sxs-lookup"><span data-stu-id="2d1cd-115">The checksum passes</span></span>

    <span data-ttu-id="2d1cd-116">In het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor een beleid van DLP Credit Card nummer:</span><span class="sxs-lookup"><span data-stu-id="2d1cd-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="2d1cd-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="2d1cd-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="2d1cd-118">Verloopt: 2-2009</span><span class="sxs-lookup"><span data-stu-id="2d1cd-118">Expires: 2/2009</span></span>

<span data-ttu-id="2d1cd-119">Zie de volgende sectie in dit artikel voor meer informatie over wat nodig voor een **Creditcardnummer is** waargenomen voor uw inhoud: [Wat de gevoelige soorten informatie zoeken voor creditcard #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="2d1cd-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="2d1cd-120">Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2d1cd-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  