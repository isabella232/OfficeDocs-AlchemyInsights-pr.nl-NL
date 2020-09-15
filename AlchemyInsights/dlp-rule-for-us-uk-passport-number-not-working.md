---
title: DLP-regel voor US/UK-paspoortnummer werkt niet
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679219"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="61c1a-102">Problemen met DLP-US/UK-paspoort nummers</span><span class="sxs-lookup"><span data-stu-id="61c1a-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="61c1a-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="61c1a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="61c1a-104">**DLP-problemen met US/UK-paspoort nummers**</span><span class="sxs-lookup"><span data-stu-id="61c1a-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="61c1a-105">Hebt u problemen met **preventie van preventie van gegevensverlies (DLP)** voor inhoud met een **US/UK-paspoortnummer** wanneer u een DLP gevoelige informatietype in O365 gebruikt?</span><span class="sxs-lookup"><span data-stu-id="61c1a-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="61c1a-106">Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor de manier waarop het DLP-beleid zoekt wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="61c1a-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="61c1a-107">Als u bijvoorbeeld een beleid voor **US/UK Passport** hebt geconfigureerd met een betrouwbaarheidsniveau van 75%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel.</span><span class="sxs-lookup"><span data-stu-id="61c1a-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="61c1a-108">**[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Negen cijfers</span><span class="sxs-lookup"><span data-stu-id="61c1a-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="61c1a-109">**[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Negen opeenvolgende cijfers</span><span class="sxs-lookup"><span data-stu-id="61c1a-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="61c1a-110">**[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen controlesom.</span><span class="sxs-lookup"><span data-stu-id="61c1a-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="61c1a-111">**[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Een DLP-beleid is 75% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="61c1a-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="61c1a-112">Met de functie Func_usa_uk_passport vindt u de inhoud die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="61c1a-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="61c1a-113">Er is een trefwoord uit Keyword_passport gevonden.</span><span class="sxs-lookup"><span data-stu-id="61c1a-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="61c1a-114">Het volgende voorbeeld wordt bijvoorbeeld geactiveerd voor het beleid voor **US/UK Passport** : US Passport Number 123456789</span><span class="sxs-lookup"><span data-stu-id="61c1a-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="61c1a-115">Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor een US/UK-paspoortnummer voor uw inhoud: [wat voor soort gevoelige informatie wordt gezocht naar het paspoortnummer van ons/VK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="61c1a-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="61c1a-116">Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?</span><span class="sxs-lookup"><span data-stu-id="61c1a-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  