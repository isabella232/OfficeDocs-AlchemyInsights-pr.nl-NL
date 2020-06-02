---
title: DLP heeft mogelijk een aangepast type nodig
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507509"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="92595-102">DLP heeft mogelijk een aangepast type nodig</span><span class="sxs-lookup"><span data-stu-id="92595-102">DLP might need a custom type</span></span>

<span data-ttu-id="92595-103">**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="92595-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="92595-104">**DLP kan een aangepast informatietype vereisen**</span><span class="sxs-lookup"><span data-stu-id="92595-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="92595-105">Met een DLP-beleid (Data Loss Prevention) u gevoelige gegevens in uw organisatie identificeren en beschermen.</span><span class="sxs-lookup"><span data-stu-id="92595-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="92595-106">In sommige scenario's moet u mogelijk uw eigen **aangepaste** gevoelige informatietype maken om de gegevens van uw organisatie te beschermen.</span><span class="sxs-lookup"><span data-stu-id="92595-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="92595-107">Uw organisatie moet bijvoorbeeld werknemers-id's of andere gegevens van werknemers identificeren en beschermen in een bepaalde indeling die specifiek is voor uw organisatie. Zie de volgende artikelen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="92595-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="92595-108">**Een ingebouwd typen gevoelige informatie aanpassen**</span><span class="sxs-lookup"><span data-stu-id="92595-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="92595-109">Als een ingebouwd gevoelig informatietype met slechts een paar aanpassingen aan uw behoeften voldoet, u [een ingebouwd gevoelige informatietype aanpassen.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="92595-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="92595-110">U bijvoorbeeld trefwoorden toevoegen of verwijderen of ondersteunend bewijs toevoegen of verwijderen, zoals een datum of adres.</span><span class="sxs-lookup"><span data-stu-id="92595-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="92595-111">**Een aangepast gevoelig informatietype maken**</span><span class="sxs-lookup"><span data-stu-id="92595-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="92595-112">Maar als u een ander type gevoelige informatie helemaal moet identificeren en beveiligen, u [een aangepast gevoelig informatietype maken](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in de gebruikersinterface van het Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="92595-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="92595-113">**Een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="92595-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="92595-114">Tot slot, als de gebruikersinterface niet alle opties biedt die u nodig hebt, u [een aangepast gevoelig informatietype maken in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="92595-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="92595-115">Door te beginnen met een XML-bestand, u elke beschikbare optie gebruiken.</span><span class="sxs-lookup"><span data-stu-id="92595-115">By starting with an XML file, you can use every option available.</span></span>
