---
title: Moderne site als de hoofdsite
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057695"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="ec982-102">Moderne site als hoofdsite</span><span class="sxs-lookup"><span data-stu-id="ec982-102">Modern site as root site</span></span>

<span data-ttu-id="ec982-103">[Release doel](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) klanten kunnen nu de moderne communicatie site ervaring op de klassieke hoofdsite van de huurder SharePoint inschakelen.</span><span class="sxs-lookup"><span data-stu-id="ec982-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="ec982-104">Deze functie kan worden geactiveerd door een eenvoudige PowerShell-cmdlet uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="ec982-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="ec982-105">Op de geslaagde uitvoering van de PowerShell--opdracht(en) moet de hoofdsite een nieuwe introductiepagina van communicatie.</span><span class="sxs-lookup"><span data-stu-id="ec982-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="ec982-106">Details over de PowerShell-cmdlet en functie-eisen zijn beschikbaar in het artikel [Inschakelen SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="ec982-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="ec982-107">We zullen worden geleidelijk rolling dit, uit standaard aan klanten gericht Release in begin mei 2019, en het doorvoeren van beschikbaar over de hele wereld aan het einde van juni 2019.</span><span class="sxs-lookup"><span data-stu-id="ec982-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="ec982-108">Doorgaan om te verwijzen naar het [Berichtencentrum](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) voor andere nieuwe functies met Modern.</span><span class="sxs-lookup"><span data-stu-id="ec982-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="ec982-109">**Belangrijk**: Verwijder de klassieke hoofdsite om een moderne communicatie-Site te maken.</span><span class="sxs-lookup"><span data-stu-id="ec982-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="ec982-110">Dit wordt niet ondersteund door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ec982-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="ec982-111">Verwijderen van de hoofdsite brengt alle SharePoint-sites in uw organisatie niet toegankelijk voor alle gebruikers, totdat u de site terugzetten of maak een nieuwe site op dezelfde URL.</span><span class="sxs-lookup"><span data-stu-id="ec982-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 