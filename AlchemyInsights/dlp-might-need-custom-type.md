---
title: DLP heeft mogelijk een aangepast type nodig
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712179"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="b77d9-102">DLP heeft mogelijk een aangepast type nodig</span><span class="sxs-lookup"><span data-stu-id="b77d9-102">DLP might need a custom type</span></span>

<span data-ttu-id="b77d9-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b77d9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b77d9-104">**Voor DLP is mogelijk een aangepast gegevenstype vereist**</span><span class="sxs-lookup"><span data-stu-id="b77d9-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="b77d9-105">Met een DLP-beleid (preventie van gegevensverlies) kunt u gevoelige gegevens in uw organisatie identificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="b77d9-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="b77d9-106">In sommige gevallen moet u mogelijk uw eigen, **aangepaste** informatietype maken om de gegevens van uw organisatie te beschermen.</span><span class="sxs-lookup"><span data-stu-id="b77d9-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="b77d9-107">Stel dat uw organisatie de Id's van werknemers of andere gegevens moet identificeren en beschermen in bepaalde indelingen, specifiek voor uw organisatie. Zie de volgende artikelen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b77d9-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="b77d9-108">**Een ingebouwd type gevoelige informatie aanpassen**</span><span class="sxs-lookup"><span data-stu-id="b77d9-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="b77d9-109">Als een ingebouwd, gevoelige informatietype aan uw wensen voldoet, kunt u [een ingebouwd gevoelige informatietype aanpassen](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="b77d9-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="b77d9-110">U kunt bijvoorbeeld trefwoorden toevoegen of verwijderen, of ondersteunend materiaal toevoegen of verwijderen, zoals een datum of adres.</span><span class="sxs-lookup"><span data-stu-id="b77d9-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="b77d9-111">**Een aangepast gevoelige informatietype maken**</span><span class="sxs-lookup"><span data-stu-id="b77d9-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="b77d9-112">Als u een ander type gevoelige informatie moet identificeren en beveiligen, kunt u [een aangepast, gevoelige informatietype maken](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in de gebruikersinterface van de beveiligings & compliance Center.</span><span class="sxs-lookup"><span data-stu-id="b77d9-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="b77d9-113">**Een aangepast, kwetsbaar informatietype maken in beveiligings & nalevings centrum voor PowerShell**</span><span class="sxs-lookup"><span data-stu-id="b77d9-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="b77d9-114">Ten slotte, als de GEBRUIKERSINTERFACE niet alle benodigde opties bevat, kunt u [een aangepast, gevoelige informatietype maken in de beveiligings & nalevings centrum voor PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b77d9-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="b77d9-115">Als u begint met een XML-bestand, kunt u alle beschikbare opties gebruiken.</span><span class="sxs-lookup"><span data-stu-id="b77d9-115">By starting with an XML file, you can use every option available.</span></span>
