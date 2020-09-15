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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694451"
---
# <a name="open-with-explorer-isnt-working"></a>Openen met Explorer werkt niet

Als **openen met Verkenner** of **weergave in de Verkenner** niet werkt, controleert u of de WebClient-service is ingesteld om te worden **uitgevoerd** door de onderstaande stappen te volgen. Het kan enige tijd duren voordat u een SharePoint-of OneDrive-bibliotheek opent wanneer de service niet actief is. 
  
1. Typ in het vak Windows Search de tekst run, selecteer de bureaublad-app uitvoeren, typ services. msc en selecteer vervolgens **Enter**.
    
2. Schuif omlaag naar de WebClient service en kijk in de kolom **status** . Als de status van de client service niet **actief**is, dubbelklikt u op de service, klikt u op **Start**en klikt u vervolgens op **OK**. Schakel de service, indien nodig, in en selecteer **handmatig** of **automatisch** in het vak **Opstarttype** . 
    
> [!NOTE]
> Zie [openen in Verkenner](https://go.microsoft.com/fwlink/?linkid=871665)voor informatie over het oplossen van problemen met openen in de Verkenner. Ontdek de synchronisatie als een beter alternatief: [SharePoint-bestanden synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

