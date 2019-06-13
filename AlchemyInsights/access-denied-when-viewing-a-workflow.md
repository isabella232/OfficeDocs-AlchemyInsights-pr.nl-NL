---
title: Toegang geweigerd bij het bekijken van een werkstroom
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883586"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="7959a-102">Toegang geweigerd bij het bekijken van een werkstroom</span><span class="sxs-lookup"><span data-stu-id="7959a-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="7959a-103">SharePoint 2013 werkstromen die probeert een e-mailbericht verzenden naar een SharePoint-groep kan mislukken met het foutbericht 'Toegang geweigerd' wordt weergegeven als het lidmaatschap van de SharePoint-groep niet is ingesteld op iedereen.</span><span class="sxs-lookup"><span data-stu-id="7959a-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="7959a-104">**Voer deze stappen uit dit probleem op te lossen:**</span><span class="sxs-lookup"><span data-stu-id="7959a-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="7959a-105">Laat iedereen zien de leden van de SharePoint-groep.</span><span class="sxs-lookup"><span data-stu-id="7959a-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="7959a-106">De SharePoint-groep verwijderen uit aan of CC regel van het e-mailbericht.</span><span class="sxs-lookup"><span data-stu-id="7959a-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="7959a-107">De gebruikers expliciet toevoegen aan het aan of CC regel als de zichtbaarheid van het lidmaatschap voor de SharePoint-groep kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="7959a-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="7959a-108">Als u wilt bekijken Zie meer details [Onbevoegde HTTP te /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7959a-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  