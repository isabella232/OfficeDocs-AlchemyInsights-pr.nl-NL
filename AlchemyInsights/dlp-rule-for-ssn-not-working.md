---
title: DLP-regel voor SSN werkt niet
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679364"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="712b3-102">DLP-problemen met sofi-nummers</span><span class="sxs-lookup"><span data-stu-id="712b3-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="712b3-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="712b3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="712b3-104">**DLP-problemen met naar ssn's**</span><span class="sxs-lookup"><span data-stu-id="712b3-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="712b3-105">Ondervindt u problemen met **preventie van gegevensverlies (DLP)** voor inhoud met een **sofi-nummer (SSN)** voor het gebruik van een type gevoelige informatie in Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="712b3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="712b3-106">Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor het opzoeken van het DLP-beleid.</span><span class="sxs-lookup"><span data-stu-id="712b3-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="712b3-107">Als u bijvoorbeeld een SSN-beleid hebt geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:</span><span class="sxs-lookup"><span data-stu-id="712b3-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="712b3-108">**[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cijfers in een opgemaakt of niet-opgemaakt patroon</span><span class="sxs-lookup"><span data-stu-id="712b3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="712b3-109">**[Patroon:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier functies zoeken naar naar ssn's met vier verschillende patronen:</span><span class="sxs-lookup"><span data-stu-id="712b3-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="712b3-110">Met Func_ssn vindt u naar ssn's met een sterke opmaak van vóór 2011, opgemaakt met streepjes of spaties (ddd-DD-dddd of ddd DD dddd)</span><span class="sxs-lookup"><span data-stu-id="712b3-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="712b3-111">Met Func_unformatted_ssn vindt u naar ssn's met een sterke opmaak van vóór 2011 die niet is opgemaakt als negen opeenvolgende cijfers (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="712b3-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="712b3-112">Met Func_randomized_formatted_ssn vindt u post-2011-naar ssn's die zijn opgemaakt met streepjes of spaties (ddd-DD-dddd of ddd DD dddd)</span><span class="sxs-lookup"><span data-stu-id="712b3-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="712b3-113">Met Func_randomized_unformatted_ssn vindt u post-2011-naar ssn's die niet zijn opgemaakt als negen opeenvolgende cijfers (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="712b3-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="712b3-114">**[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nee, er is geen controlesom.</span><span class="sxs-lookup"><span data-stu-id="712b3-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="712b3-115">**[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Een DLP-beleid is 85% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="712b3-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="712b3-116">Met de [functie Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) vindt u de inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="712b3-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="712b3-117">Er is een trefwoord uit [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) gevonden.</span><span class="sxs-lookup"><span data-stu-id="712b3-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="712b3-118">Voorbeelden van trefwoorden  *zijn: Social Security, Social Security #, SOC sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="712b3-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="712b3-119">Het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor het DLP-SSN-beleid: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="712b3-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="712b3-120">Zie de volgende sectie in dit artikel voor meer informatie over de vereisten voor naar ssn's voor uw inhoud: de [typen gevoelige informatie zoekt](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) u naar naar ssn's</span><span class="sxs-lookup"><span data-stu-id="712b3-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="712b3-121">Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?</span><span class="sxs-lookup"><span data-stu-id="712b3-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  