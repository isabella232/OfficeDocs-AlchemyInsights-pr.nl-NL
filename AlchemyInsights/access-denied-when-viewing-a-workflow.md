---
title: Toegang geweigerd bij het weergeven van een werkstroom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688797"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="be7f6-102">Toegang geweigerd bij het weergeven van een werkstroom</span><span class="sxs-lookup"><span data-stu-id="be7f6-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="be7f6-103">SharePoint 2013-werkstromen die een e-mailbericht verzenden naar een SharePoint-groep, kunnen niet worden geopend met een foutbericht ' toegang geweigerd ' als het lidmaatschap van de SharePoint-groep niet is ingesteld op iedereen.</span><span class="sxs-lookup"><span data-stu-id="be7f6-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="be7f6-104">**Voer de volgende stappen uit om dit probleem op te lossen:**</span><span class="sxs-lookup"><span data-stu-id="be7f6-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="be7f6-105">Iedereen toestaan de leden van de SharePoint-groep te zien.</span><span class="sxs-lookup"><span data-stu-id="be7f6-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="be7f6-106">Verwijder de SharePoint-groep van de regel aan of CC van het e-mailbericht.</span><span class="sxs-lookup"><span data-stu-id="be7f6-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="be7f6-107">U kunt de gebruikers expliciet toevoegen aan de regel aan of CC als de zichtbaarheid van het lidmaatschap van de SharePoint-groep niet kan worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="be7f6-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="be7f6-108">Voor meer informatie raadpleegt u [http authorized to/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="be7f6-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  