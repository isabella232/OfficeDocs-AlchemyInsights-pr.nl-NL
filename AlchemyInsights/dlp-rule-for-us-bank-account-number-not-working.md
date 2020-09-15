---
title: DLP-regel voor US Bank-account nummer werkt niet
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679291"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="2c6f5-102">DLP-problemen met US bankrekening nummers</span><span class="sxs-lookup"><span data-stu-id="2c6f5-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="2c6f5-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2c6f5-104">**DLP-problemen met US bankrekening nummers**</span><span class="sxs-lookup"><span data-stu-id="2c6f5-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="2c6f5-105">Hebt u problemen met **preventie van preventie van gegevensverlies (DLP)** voor inhoud met een **account van een Amerikaanse bank rekening** wanneer u een DLP gevoelige informatietype in O365 gebruikt?</span><span class="sxs-lookup"><span data-stu-id="2c6f5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2c6f5-106">Als dit het geval is, moet u ervoor zorgen dat de inhoud de benodigde informatie bevat voor de manier waarop het DLP-beleid zoekt wanneer het wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2c6f5-107">Voor het **account nummer van een US Bank** is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden de volgende stappen geëvalueerd en moet de regel worden geactiveerd voor de regel:</span><span class="sxs-lookup"><span data-stu-id="2c6f5-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2c6f5-108">**[Notatie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cijfers</span><span class="sxs-lookup"><span data-stu-id="2c6f5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="2c6f5-109">**[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 opeenvolgende cijfers.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="2c6f5-110">**[Controlesom:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen controlesom.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2c6f5-111">**[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Een DLP-beleid is 75% zekerheid dat dit type gevoelige informatie is gedetecteerd als binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="2c6f5-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2c6f5-112">Met de reguliere expressie Regex_usa_bank_account_number u inhoud vindt die overeenkomt met het patroon.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="2c6f5-113">Er is een trefwoord uit Keyword_usa_Bank_Account gevonden.</span><span class="sxs-lookup"><span data-stu-id="2c6f5-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="2c6f5-114">Met het volgende voorbeeld wordt bijvoorbeeld het 78344011 beleid voor het **accountnummer** van uw account in de VS</span><span class="sxs-lookup"><span data-stu-id="2c6f5-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="2c6f5-115">Zie de volgende sectie in dit artikel voor meer informatie over wat er is vereist voor de inhoud van uw account in de **Verenigde Staten** : met [de typen gevoelige informatie wordt gezocht naar het accountnummer van de Amerikaanse bank](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .</span><span class="sxs-lookup"><span data-stu-id="2c6f5-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="2c6f5-116">Raadpleeg het volgende artikel voor informatie over wat er is vereist voor andere typen: [waar de typen gevoelige informatie op letten](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) ?</span><span class="sxs-lookup"><span data-stu-id="2c6f5-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  