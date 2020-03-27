---
title: DLP-regel voor paspoortnummer VS/VK werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977101"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="ccc26-102">Problemen met DLP - Paspoortnummers VS/VK</span><span class="sxs-lookup"><span data-stu-id="ccc26-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="ccc26-103">**Belangrijk:** Tijdens deze ongekende tijden nemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services zeer beschikbaar blijven - Ga naar [tijdelijke functieaanpassingen van SharePoint Online](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ccc26-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ccc26-104">**DLP problemen met de VS / UK paspoortnummers**</span><span class="sxs-lookup"><span data-stu-id="ccc26-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="ccc26-105">Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **paspoortnummer tussen de VS en het VK** bevat bij het gebruik van een DLP-gevoelig informatietype in O365?</span><span class="sxs-lookup"><span data-stu-id="ccc26-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ccc26-106">Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="ccc26-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ccc26-107">Voor een **paspoortnummerbeleid tussen de VS en het VK** dat is geconfigureerd met een betrouwbaarheidsniveau van 75%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd om de regel te activeren</span><span class="sxs-lookup"><span data-stu-id="ccc26-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="ccc26-108">**[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Negen cijfers</span><span class="sxs-lookup"><span data-stu-id="ccc26-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="ccc26-109">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Negen opeenvolgende cijfers</span><span class="sxs-lookup"><span data-stu-id="ccc26-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="ccc26-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen Checksum</span><span class="sxs-lookup"><span data-stu-id="ccc26-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ccc26-111">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Een DLP-beleid is 75% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="ccc26-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ccc26-112">De functie Func_usa_uk_passport vindt inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="ccc26-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ccc26-113">Er wordt een trefwoord uit Keyword_passport gevonden.</span><span class="sxs-lookup"><span data-stu-id="ccc26-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="ccc26-114">De volgende steekproef zou bijvoorbeeld leiden tot het beleid van het paspoortnummer tussen de **VS en het Verenigd Koninkrijk:** Amerikaans paspoortnummer 123456789</span><span class="sxs-lookup"><span data-stu-id="ccc26-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="ccc26-115">Zie de volgende sectie in dit artikel voor meer informatie over wat er nodig is om een paspoortnummer tussen de VS en het VK te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar het paspoortnummer tussen de VS en het Vk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ccc26-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ccc26-116">Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ccc26-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  