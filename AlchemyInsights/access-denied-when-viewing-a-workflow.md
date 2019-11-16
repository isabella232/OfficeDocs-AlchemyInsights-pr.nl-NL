---
title: Toegang geweigerd bij het bekijken van een workflow
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747743"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="713d9-102">Toegang geweigerd bij het bekijken van een workflow</span><span class="sxs-lookup"><span data-stu-id="713d9-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="713d9-103">SharePoint 2013-werkstromen die proberen te verzenden van een e-mail bericht naar een SharePoint-groep kan mislukken met een ' toegang geweigerd ' foutmelding als het lidmaatschap van de SharePoint-groep niet is ingesteld op iedereen.</span><span class="sxs-lookup"><span data-stu-id="713d9-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="713d9-104">**Voer de volgende stappen uit om dit probleem op te lossen:**</span><span class="sxs-lookup"><span data-stu-id="713d9-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="713d9-105">Laat iedereen de leden van de SharePoint-groep zien.</span><span class="sxs-lookup"><span data-stu-id="713d9-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="713d9-106">Verwijder de SharePoint-groep van de regel aan of CC van de e-mail.</span><span class="sxs-lookup"><span data-stu-id="713d9-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="713d9-107">Voeg de gebruikers expliciet toe aan de regel aan of CC als de zichtbaarheid van het lidmaatschap niet kan worden gewijzigd voorsharepoint Group.</span><span class="sxs-lookup"><span data-stu-id="713d9-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="713d9-108">Voor meer informatie verwijzen wij u naar [http ongeautoriseerde aan/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="713d9-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  