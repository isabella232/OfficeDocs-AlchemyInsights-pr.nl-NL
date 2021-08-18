---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321856"
---
# <a name="open-with-explorer-isnt-working"></a>Openen met Explorer werkt niet

Als **Openen met Verkenner** of Weergave **in** Verkenner niet werkt, moet u ervoor zorgen dat de WebClient-service is ingesteld op Uitvoeren **door** de onderstaande stappen te volgen. Het kan bijvoorbeeld lang duren voordat een bibliotheek SharePoint of OneDrive wordt geopend wanneer de service niet wordt uitgevoerd. 
  
1. Typ in Windows zoekvak Uitvoeren, selecteer de bureaublad-app Uitvoeren, typ services.msc en selecteer **vervolgens Enter**.
    
2. Schuif omlaag naar de WebClient-service en controleer de **kolom** Status. Als de WebClient-servicestatus niet **wordt uitgevoerd,** dubbelklikt u op de service, klikt u op **Start** en klikt u vervolgens op **OK.** Schakel de service indien nodig in door Handmatig **of** Automatisch in **het** vak Type opstarten **te** selecteren. 
    
**Opmerking:** Zie Openen in Verkenner als u problemen met het openen van bestanden in Verkenner [wilt oplossen.](https://go.microsoft.com/fwlink/?linkid=871665) Synchronisatie verkennen als een beter alternatief: [Synchroniseer SharePoint bestanden met de nieuwe OneDrive-synchronisatie client.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

