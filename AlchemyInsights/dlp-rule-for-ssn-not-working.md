---
title: DLP-regel voor het sofi-nummer niet werkt
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404412"
---
<span data-ttu-id="3847f-102">Ondervindt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud met een **Sofi-nummer (Sofinummer)** bij gebruik van een type vertrouwelijke informatie in Office 365?</span><span class="sxs-lookup"><span data-stu-id="3847f-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="3847f-103">Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor wat het DLP-beleid is op zoek.</span><span class="sxs-lookup"><span data-stu-id="3847f-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="3847f-104">Bijvoorbeeld voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, het volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren:</span><span class="sxs-lookup"><span data-stu-id="3847f-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3847f-105">**[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cijfers bestaan, die mogelijk in een geformatteerde of ongeformatteerde patroon</span><span class="sxs-lookup"><span data-stu-id="3847f-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="3847f-106">**[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken voor SSNs in vier verschillende patronen:</span><span class="sxs-lookup"><span data-stu-id="3847f-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="3847f-107">Func_ssn zoekt SSNs met pre-2011 sterke opmaak die zijn opgemaakt met streepjes of ruimten (ddd-dd-dddd of ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="3847f-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="3847f-108">Func_unformatted_ssn zoekt SSNs met pre-2011 sterke opmaak die zijn geformatteerd als negen opeenvolgende cijfers (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="3847f-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="3847f-109">Func_randomized_formatted_ssn boeken-2011-SSNs die zijn opgemaakt met streepjes of ruimten (ddd-dd-dddd of ddd dd dddd) wordt gevonden</span><span class="sxs-lookup"><span data-stu-id="3847f-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="3847f-110">Func_randomized_unformatted_ssn zoekt boeken 2011-SSNs die geformatteerd als negen opeenvolgende cijfers (ddddddddd zijn)</span><span class="sxs-lookup"><span data-stu-id="3847f-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="3847f-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nee, er is geen controlesom</span><span class="sxs-lookup"><span data-stu-id="3847f-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="3847f-112">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="3847f-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3847f-113">De [functie Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) wordt gezocht naar inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="3847f-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="3847f-114">Een sleutelwoord [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is gevonden.</span><span class="sxs-lookup"><span data-stu-id="3847f-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="3847f-115">Bevat voorbeelden van trefwoorden: *sociale zekerheid, sociale zekerheid #, Werknemerspremies, sofi-nummer* .</span><span class="sxs-lookup"><span data-stu-id="3847f-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="3847f-116">Zoals in het volgende voorbeeld wordt voor de SSN DLP-beleid: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="3847f-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="3847f-117">Zie de volgende sectie in dit artikel voor meer informatie over wat is vereist voor SSNs voor uw inhoud worden gedetecteerd: [Wat de gevoelige soorten informatie zoekt SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="3847f-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="3847f-118">Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3847f-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

