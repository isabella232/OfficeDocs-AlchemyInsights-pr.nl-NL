---
title: Openen met Explorer werkt niet
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713029"
---
# <a name="open-with-explorer-isnt-working"></a>Openen met Explorer werkt niet

Als **Openen met Verkenner** of Weergave in **Verkenner** niet werkt, moet u ervoor zorgen dat de WebClient-service is ingesteld op **Uitvoeren** door de onderstaande stappen te volgen. Het kan bijvoorbeeld lang duren voordat een SharePoint- of OneDrive-bibliotheek is geopend wanneer de service niet wordt uitgevoerd. 
  
1. Typ in het zoekvak van Windows uitvoeren, selecteer de bureaublad-app uitvoeren, typ services.msc en selecteer **Enter**.
    
2. Schuif omlaag naar de WebClient-service en controleer de kolom **Status.** Als de status van de WebClient-service niet **wordt uitgevoerd,** dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**. Schakel de service indien nodig in door **Handmatig** of **automatisch** te selecteren in het vak **Opstarttype.** 
    
> [!NOTE]
> Zie [Openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor het oplossen van problemen in Verkenner. Synchronisatie verkennen als een beter alternatief: [SharePoint-bestanden synchroniseren met de nieuwe Synchronisatieclient van OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

