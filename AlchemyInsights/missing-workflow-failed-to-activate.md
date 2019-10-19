---
title: Ontbrekende werkstroom kan niet worden geactiveerd
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753791"
---
# <a name="missing-workflow-failed-to-activate"></a>Ontbrekende werkstroom kan niet worden geactiveerd

In een Microsoft SharePoint-siteverzameling u een globaal herbruikbare werkstroom (zoals ' goedkeuring-SharePoint 2010 ') niet toevoegen aan een lijst of bibliotheek.
  
Voer de volgende stappen uit om dit probleem op te lossen: 
  
1. Open de hoofdwebsite van de siteverzameling in SharePoint Designer 2013.
  
2. Onder **site objecten**, selecteer **Werkstromen**. 
  
3. Selecteer in de sectie **Nieuw** van het lint **Werkstromen** **herbruikbare werkstroom**. 
  
4. Voer op het formulier **herbruikbare werkstroom maken** de naam * * *Repair2010* * * in. Voor **platform type**, klikt u op **SharePoint 2010 workflow**en klik vervolgens op **OK**. 
  
1. In de **Opslaan** sectie van de **werkstroom** lint, selecteer **publiceren**. 
  
2. In de **beheren** sectie van de **werkstroom** lint, selecteer **wereldwijd publiceren**. Selecteer **OK**in het bevestigingsdialoogvenster dat verschijnt. 
  
3. Zoek in een webbrowser de hoofdwebsite van de siteverzameling en vervolgens toegang tot site- **instellingen** \> **siteverzameling functies**. Schakel vervolgens de functie **workflows** in: 
  
· Als de functie is *geactiveerd* , klikt u op **deactiveren** en vervolgens op **activeren**. 
  
· Als de functie is *gedeactiveerd* , klikt u op **activeren**. 
  
Raadpleeg het volgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)voor meer informatie.
  

