---
title: DLP-regel voor SSN werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704080"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="83481-102">DLP problemen met sofinummers</span><span class="sxs-lookup"><span data-stu-id="83481-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="83481-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="83481-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="83481-104">**DLP-problemen met SSN's**</span><span class="sxs-lookup"><span data-stu-id="83481-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="83481-105">Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **SSN (Social Security Number)** bevat bij het gebruik van een gevoelig informatietype in Office 365?</span><span class="sxs-lookup"><span data-stu-id="83481-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="83481-106">Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt.</span><span class="sxs-lookup"><span data-stu-id="83481-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="83481-107">Voor een SSN-beleid dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:</span><span class="sxs-lookup"><span data-stu-id="83481-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="83481-108">**[Opmaak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cijfers, die zich in een opgemaakt of niet-opgemaakt patroon kunnen begeven</span><span class="sxs-lookup"><span data-stu-id="83481-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="83481-109">**[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar SSN's in vier verschillende patronen:</span><span class="sxs-lookup"><span data-stu-id="83481-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="83481-110">Func_ssn vindt SSN's met een sterke opmaak van voor 2011 die zijn opgemaakt met streepjes of spaties (ddd-dddd of ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="83481-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="83481-111">Func_unformatted_ssn vindt SSN's met een sterke opmaak van voor 2011 die niet zijn opgemaakt als negen opeenvolgende cijfers (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="83481-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="83481-112">Func_randomized_formatted_ssn vindt ssn's na 2011 die zijn opgemaakt met streepjes of spaties (ddd-dddd of ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="83481-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="83481-113">Func_randomized_unformatted_ssn vindt ssn na 2011 zonder opmaak als negen opeenvolgende cijfers (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="83481-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="83481-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nee, er is geen Checksum</span><span class="sxs-lookup"><span data-stu-id="83481-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="83481-115">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Een DLP-beleid is 85% ervan overtuigd dat het dit soort gevoelige informatie heeft gedetecteerd als, binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="83481-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="83481-116">De [functie Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) vindt inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="83481-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="83481-117">Er wordt een trefwoord uit [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) gevonden.</span><span class="sxs-lookup"><span data-stu-id="83481-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="83481-118">Voorbeelden van trefwoorden zijn: *Sociale Zekerheid, Sociale Zekerheid#, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="83481-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="83481-119">De volgende steekproef wordt bijvoorbeeld geactiveerd voor het DLP SSN-beleid: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="83481-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="83481-120">Zie het volgende gedeelte in dit artikel [voor](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn) meer informatie over wat er nodig is om SSN's te detecteren voor uw inhoud.</span><span class="sxs-lookup"><span data-stu-id="83481-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="83481-121">Zie het volgende artikel voor informatie over wat er nodig is voor andere typen: [Waar de gevoelige informatietypen naar zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="83481-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  