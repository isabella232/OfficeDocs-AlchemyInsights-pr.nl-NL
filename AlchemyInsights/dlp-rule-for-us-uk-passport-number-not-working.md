---
title: DLP-regel voor de Verenigde Staten / Verenigd Koninkrijk paspoortnummer werkt niet
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912091"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="72f46-102">Problemen met DLP - US / UK Passport getallen</span><span class="sxs-lookup"><span data-stu-id="72f46-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="72f46-p101">Hebt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud die een **VS / VK paspoortnummer** wanneer u een type DLP gevoelige informatie in O365? Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor wat het DLP-beleid is op zoek naar wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="72f46-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="72f46-105">Bijvoorbeeld voor een **VS / VK paspoortnummer** beleid is geconfigureerd met een betrouwbaarheidsniveau van 75%, de volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren</span><span class="sxs-lookup"><span data-stu-id="72f46-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="72f46-106">**[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Negen cijfers</span><span class="sxs-lookup"><span data-stu-id="72f46-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="72f46-107">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Negen opeenvolgende cijfers</span><span class="sxs-lookup"><span data-stu-id="72f46-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="72f46-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen controlesom</span><span class="sxs-lookup"><span data-stu-id="72f46-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="72f46-109">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Een DLP-beleid is 75% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="72f46-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="72f46-110">De functie Func_usa_uk_passport wordt gezocht naar inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="72f46-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="72f46-111">Een sleutelwoord Keyword_passport is gevonden.</span><span class="sxs-lookup"><span data-stu-id="72f46-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="72f46-112">Zoals in het volgende voorbeeld wordt voor de **VS / VK paspoortnummer** beleid: Amerikaans paspoort getal 123456789</span><span class="sxs-lookup"><span data-stu-id="72f46-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="72f46-113">Voor meer informatie over wat nodig voor een Amerikaanse is / paspoortnummer UK waargenomen voor uw inhoud, Zie de volgende sectie in dit artikel: [Wat de gevoelige soorten informatie uiterlijk voor Amerikaanse / paspoortnummer UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="72f46-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="72f46-114">Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="72f46-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

