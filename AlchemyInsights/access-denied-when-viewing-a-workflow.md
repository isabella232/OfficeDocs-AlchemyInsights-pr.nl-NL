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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747743"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Toegang geweigerd bij het bekijken van een workflow

SharePoint 2013-werkstromen die proberen te verzenden van een e-mail bericht naar een SharePoint-groep kan mislukken met een ' toegang geweigerd ' foutmelding als het lidmaatschap van de SharePoint-groep niet is ingesteld op iedereen.
  
 **Voer de volgende stappen uit om dit probleem op te lossen:**
  
 1. Laat iedereen de leden van de SharePoint-groep zien.
  
 2. Verwijder de SharePoint-groep van de regel aan of CC van de e-mail.
  
 3. Voeg de gebruikers expliciet toe aan de regel aan of CC als de zichtbaarheid van het lidmaatschap niet kan worden gewijzigd voorsharepoint Group.
  
Voor meer informatie verwijzen wij u naar [http ongeautoriseerde naar/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  