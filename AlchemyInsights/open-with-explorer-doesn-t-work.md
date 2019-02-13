---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906799"
---
# <a name="open-with-explorer-isnt-working"></a>Openen met Explorer werkt niet

Als **openen met Explorer** of **weergave in File Explorer** werkt niet controleren of dat de WebClient-service is ingesteld op **wordt uitgevoerd** door de onderstaande stappen te volgen. Het duurt zo lang voor het openen van een documentbibliotheek van SharePoint of OneDrive als de service niet wordt uitgevoerd. 
  
1. Selecteer in het zoekvak van Windows, type uitvoert, de desktop app Run, type services.msc en klik vervolgens op **Enter**.
    
2. Blader naar de WebClient-service en de kolom **Status** . Als de status van de WebClient-service niet **wordt uitgevoerd**, dubbelklikt u op de service, klikt u op **Start**en klik vervolgens op **OK**. Schakel de service, als deze nodig zijn, **handmatig** of **automatisch** selecteren in het vak **Opstarttype** . 
    
> [!NOTE]
> Zie [openen in Explorer](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in File Explorer te openen. Ontdek synchroniseren als een beter alternatief: [Sync SharePoint-bestanden met de nieuwe OneDrive synchronisatie-client](https://go.microsoft.com/fwlink/?linkid=871666). 
  

