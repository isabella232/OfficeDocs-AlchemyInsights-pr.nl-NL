---
title: Kan 2010 goedkeuringsworkflow niet toevoegen
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049548"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Kan 2010 goedkeuringsworkflow niet toevoegen

In een Microsoft SharePoint-siteverzameling u een globaal herbruikbare werkstroom (zoals ' goedkeuring-SharePoint 2010 ') niet toevoegen aan een lijst of bibliotheek.
  
Voer de volgende stappen uit om dit probleem op te lossen: 
  
1. Open de hoofdwebsite van de siteverzameling in SharePoint Designer 2013.
  
2. Onder **site objecten**, selecteer **Werkstromen**. 
  
3. Selecteer in de sectie **Nieuw** van het lint **Werkstromen** **herbruikbare werkstroom**. 
  
4. Voer op het formulier **herbruikbare werkstroom maken** de naam * * *Repair2010* * * in. Voor **platform type**, klikt u op **SharePoint 2010 workflow**en klik vervolgens op **OK**. 
  
1. In de **Opslaan** sectie van de **werkstroom** lint, selecteer **publiceren**. 
  
2. In de **beheren** sectie van de **werkstroom** lint, selecteer **wereldwijd publiceren**. Selecteer **OK**in het bevestigingsdialoogvenster dat verschijnt. 
  
3. Zoek in een webbrowser de hoofdwebsite van de siteverzameling en vervolgens toegang tot site- **instellingen** \> **siteverzameling functies**. Schakel de functie **workflows** uit: 
  
· Als de functie is *geactiveerd* , klikt u op **deactiveren** en vervolgens op **activeren**. 
  
· Als de functie is *gedeactiveerd* , klikt u op **activeren**. 
  
Raadpleeg het volgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)voor meer informatie.
  

