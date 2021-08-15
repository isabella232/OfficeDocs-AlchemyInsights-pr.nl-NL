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
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955196"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Toegang geweigerd bij het weergeven van een werkstroom

SharePoint 2013 Werkstromen die proberen een e-mail naar een SharePoint-groep te verzenden, kunnen mislukken met een foutbericht 'Toegang geweigerd' als het lidmaatschap van de groep SharePoint niet is ingesteld op Iedereen.
  
 **Ga als volgende stappen te werk om dit probleem op te lossen:**
  
 1. Iedereen toestaan de leden van de groep SharePoint zien.
  
 2. Verwijder de SharePoint groep uit de regel Aan of CC van het e-mailbericht.
  
 3. Voeg de gebruikers expliciet toe aan de regel Aan of CC als de zichtbaarheid van het lidmaatschap niet kan worden gewijzigd voor SharePoint groep.
  
Raadpleeg HTTP Onbevoegden naar [/_vti_bin/client.svc/sp.utilities.utility.sendEmail voor](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)meer informatie.
  