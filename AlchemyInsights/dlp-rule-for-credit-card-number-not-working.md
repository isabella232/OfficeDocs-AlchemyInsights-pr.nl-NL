---
title: DLP-regel voor creditcardnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679436"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="15ec0-102">DLP-problemen met creditcardnummers</span><span class="sxs-lookup"><span data-stu-id="15ec0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="15ec0-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="15ec0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="15ec0-104">**DLP-problemen met creditcardnummers**</span><span class="sxs-lookup"><span data-stu-id="15ec0-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="15ec0-105">Ondervindt u problemen met **preventie van gegevensverlies (DLP)** voor inhoud met een **creditcardnummer** wanneer u een DLP gevoelige informatietype in O365 gebruikt?</span><span class="sxs-lookup"><span data-stu-id="15ec0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="15ec0-106">Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat om het DLP-beleid te activeren wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="15ec0-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="15ec0-107">Als u bijvoorbeeld een **creditcard beleid** hebt geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:</span><span class="sxs-lookup"><span data-stu-id="15ec0-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="15ec0-108">**[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cijfers die wel of niet zijn opgemaakt (dddddddddddddddd) en de Luhn-test moeten doorlopen.</span><span class="sxs-lookup"><span data-stu-id="15ec0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="15ec0-109">**[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zeer complex en krachtig patroon voor het detecteren van kaarten van alle belangrijkste merken wereldwijd, waaronder Visa, MasterCard, Discover Card, JCB, American Express, cadeau kaarten en diner's cards.</span><span class="sxs-lookup"><span data-stu-id="15ec0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="15ec0-110">**[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, de Luhn-controlesom</span><span class="sxs-lookup"><span data-stu-id="15ec0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="15ec0-111">**[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Een DLP-beleid is 85% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="15ec0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="15ec0-112">Met de functie Func_credit_card vindt u de inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="15ec0-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="15ec0-113">Een van de volgende beweringen is waar:</span><span class="sxs-lookup"><span data-stu-id="15ec0-113">One of the following is true:</span></span>

  - <span data-ttu-id="15ec0-114">Er is een trefwoord uit Keyword_cc_verification gevonden.</span><span class="sxs-lookup"><span data-stu-id="15ec0-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="15ec0-115">Een trefwoord uit Keyword_cc_name wordt gevonden</span><span class="sxs-lookup"><span data-stu-id="15ec0-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="15ec0-116">Met de functie Func_expiration_date vindt u een datum in de juiste datumnotatie.</span><span class="sxs-lookup"><span data-stu-id="15ec0-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="15ec0-117">De checksum verstuurt</span><span class="sxs-lookup"><span data-stu-id="15ec0-117">The checksum passes</span></span>

    <span data-ttu-id="15ec0-118">Met het volgende voorbeeld wordt bijvoorbeeld het beleid voor DLP-creditcardnummers geactiveerd:</span><span class="sxs-lookup"><span data-stu-id="15ec0-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="15ec0-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="15ec0-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="15ec0-120">Verloopt over: 2/2009</span><span class="sxs-lookup"><span data-stu-id="15ec0-120">Expires: 2/2009</span></span>

<span data-ttu-id="15ec0-121">Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor een **creditcardnummer** ter detectie van uw inhoud: [wat voor soort gevoelige informatie wordt weergegeven op een creditcard #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="15ec0-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="15ec0-122">Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?</span><span class="sxs-lookup"><span data-stu-id="15ec0-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  