---
title: DLP-regel voor bankrekeningnummer VS werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507329"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="0e570-102">DLP-problemen met bankrekeningnummers vs</span><span class="sxs-lookup"><span data-stu-id="0e570-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="0e570-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0e570-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0e570-104">**DLP-problemen met bankrekeningnummers vs**</span><span class="sxs-lookup"><span data-stu-id="0e570-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="0e570-105">Heeft u problemen met **Data Loss Prevention (DLP)** die niet werkt voor inhoud die een **Amerikaans bankrekeningnummer** bevat bij het gebruik van een DLP-gevoelig informatietype in O365?</span><span class="sxs-lookup"><span data-stu-id="0e570-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0e570-106">Zorg er dan voor dat uw inhoud de benodigde informatie bevat voor wat het DLP-beleid zoekt wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="0e570-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0e570-107">Voor een beleid voor **een Amerikaans bankrekeningnummer** dat is geconfigureerd met een betrouwbaarheidsniveau van 85%, worden bijvoorbeeld de volgende geëvalueerd en moet worden gedetecteerd voordat de regel kan worden geactiveerd:</span><span class="sxs-lookup"><span data-stu-id="0e570-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0e570-108">**[Opmaak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cijfers</span><span class="sxs-lookup"><span data-stu-id="0e570-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="0e570-109">**[Patroon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 opeenvolgende cijfers.</span><span class="sxs-lookup"><span data-stu-id="0e570-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="0e570-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nee, er is geen Checksum</span><span class="sxs-lookup"><span data-stu-id="0e570-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0e570-111">**[Definitie:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Een DLP-beleid is er 75% van overtuigd dat dit soort gevoelige informatie wordt gedetecteerd als, binnen een nabijheid van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="0e570-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0e570-112">De reguliere expressie Regex_usa_bank_account_number vindt inhoud die overeenkomt met het patroon</span><span class="sxs-lookup"><span data-stu-id="0e570-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="0e570-113">Er wordt een trefwoord uit Keyword_usa_Bank_Account gevonden.</span><span class="sxs-lookup"><span data-stu-id="0e570-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="0e570-114">De volgende steekproef wordt bijvoorbeeld geactiveerd voor het beleid voor **bankrekeningnummer van** de VS: Betaalrekening 78344011</span><span class="sxs-lookup"><span data-stu-id="0e570-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="0e570-115">Zie het volgende gedeelte in dit artikel voor meer informatie over wat er nodig is om een **Amerikaans bankrekeningnummer** te detecteren voor uw inhoud: [Wat de gevoelige informatietypen zoeken naar bankrekeningnummer van de VS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="0e570-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="0e570-116">Zie het volgende artikel met behulp van een ander ingebouwd type gevoelige informatie voor informatie over wat nodig is voor andere typen: [Waar de typen gevoelige informatie naar zoeken](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0e570-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  