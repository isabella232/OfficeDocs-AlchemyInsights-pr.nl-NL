---
title: Toegang geweigerd bij het bekijken van een werkstroom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687325"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a609d-102">Toegang geweigerd bij het bekijken van een werkstroom</span><span class="sxs-lookup"><span data-stu-id="a609d-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a609d-103">SharePoint 2013-werkstromen die proberen een e-mail naar een SharePoint-groep te verzenden, kunnen mislukken met een foutbericht 'Toegang geweigerd' als het lidmaatschap van de SharePoint-groep niet is ingesteld op Iedereen.</span><span class="sxs-lookup"><span data-stu-id="a609d-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a609d-104">**Ga als volgt te werk om dit probleem op te lossen:**</span><span class="sxs-lookup"><span data-stu-id="a609d-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a609d-105">Laat iedereen de leden van de SharePoint-groep zien.</span><span class="sxs-lookup"><span data-stu-id="a609d-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="a609d-106">Verwijder de SharePoint-groep uit de aan- of CC-regel van de e-mail.</span><span class="sxs-lookup"><span data-stu-id="a609d-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="a609d-107">Voeg de gebruikers expliciet toe aan de aan- of CC-regel als de zichtbaarheid van het lidmaatschap niet kan worden gewijzigd voor sharepoint-groep.</span><span class="sxs-lookup"><span data-stu-id="a609d-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="a609d-108">Voor meer informatie verwijzen wij u naar [HTTP Ongeautoriseerd naar /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a609d-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  