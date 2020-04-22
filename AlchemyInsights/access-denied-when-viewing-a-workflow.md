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
# <a name="access-denied-when-viewing-a-workflow"></a>Toegang geweigerd bij het bekijken van een werkstroom

SharePoint 2013-werkstromen die proberen een e-mail naar een SharePoint-groep te verzenden, kunnen mislukken met een foutbericht 'Toegang geweigerd' als het lidmaatschap van de SharePoint-groep niet is ingesteld op Iedereen.
  
 **Ga als volgt te werk om dit probleem op te lossen:**
  
 1. Laat iedereen de leden van de SharePoint-groep zien.
  
 2. Verwijder de SharePoint-groep uit de aan- of CC-regel van de e-mail.
  
 3. Voeg de gebruikers expliciet toe aan de aan- of CC-regel als de zichtbaarheid van het lidmaatschap niet kan worden gewijzigd voor sharepoint-groep.
  
Voor meer informatie verwijzen wij u naar [HTTP Ongeautoriseerd naar /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  