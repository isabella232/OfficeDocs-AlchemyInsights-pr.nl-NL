---
title: DLP-regel voor ons bankrekeningnummer werkt niet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529857"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="0a4f5-102">Problemen met ons bankrekeningnummers DLP</span><span class="sxs-lookup"><span data-stu-id="0a4f5-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="0a4f5-103">Ondervindt u problemen met **Gegevens verlies te voorkomen (DLP)** werkt niet voor inhoud met een **Amerikaanse bankrekeningnummer** wanneer u een type DLP gevoelige informatie in O365?</span><span class="sxs-lookup"><span data-stu-id="0a4f5-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0a4f5-104">Als dat zo is, zorg ervoor dat uw inhoud bevat de benodigde informatie voor wat het DLP-beleid is op zoek naar wanneer deze wordt geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="0a4f5-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0a4f5-105">Bijvoorbeeld voor een **Amerikaanse Bank Account Number** beleid is geconfigureerd met een betrouwbaarheidsniveau van 85%, het volgende worden geëvalueerd en moet worden vastgesteld voor de regel te activeren:</span><span class="sxs-lookup"><span data-stu-id="0a4f5-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0a4f5-106">**[Indeling:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cijfers</span><span class="sxs-lookup"><span data-stu-id="0a4f5-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="0a4f5-107">**[Patroon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 opeenvolgende cijfers.</span><span class="sxs-lookup"><span data-stu-id="0a4f5-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="0a4f5-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nee, er is geen controlesom</span><span class="sxs-lookup"><span data-stu-id="0a4f5-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0a4f5-109">**[Definitie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Een DLP-beleid is 75% ervan overtuigd dat zij dit soort gevoelige gegevens heeft gedetecteerd als binnen een afstand van 300 tekens:</span><span class="sxs-lookup"><span data-stu-id="0a4f5-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0a4f5-110">De gewone uitdrukking Regex_usa_bank_account_number vindt u inhoud die overeenkomt met het patroon</span><span class="sxs-lookup"><span data-stu-id="0a4f5-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="0a4f5-111">Een sleutelwoord Keyword_usa_Bank_Account is gevonden.</span><span class="sxs-lookup"><span data-stu-id="0a4f5-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="0a4f5-112">Zoals in het volgende voorbeeld wordt voor het beleid van de **Amerikaanse Bank Account Number** : 78344011 betaalrekening</span><span class="sxs-lookup"><span data-stu-id="0a4f5-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="0a4f5-113">Zie de volgende sectie in dit artikel voor meer informatie over wat nodig voor een **Amerikaanse Bank Account Number is** waargenomen voor uw inhoud: [Wat de gevoelige soorten informatie zoeken voor een Amerikaanse Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="0a4f5-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="0a4f5-114">Het volgende artikel voor meer informatie van wat is vereist voor andere typen met behulp van een type verschillende ingebouwde gevoelige informatie, Zie: [Wat de gevoelige soorten informatie zoeken](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0a4f5-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  