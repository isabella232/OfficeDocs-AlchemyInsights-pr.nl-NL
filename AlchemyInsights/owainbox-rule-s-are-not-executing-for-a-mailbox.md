---
title: 1332 OWA - postvak (s) worden niet uitgevoerd voor een postbus
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784337"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Een regel voor postvak in werkt niet zoals verwacht

Controleer of de volgende instellingen:
  
- Een bericht kan worden omgeleid, doorgestuurd of beantwoord automatisch op basis van regels voor postvak in slechts één keer. Een omleiding regel (regel voor het postvak of e-mailregel stroom, ook bekend als een regel vervoer) kan een maximum van tien doorsturen geadresseerden toevoegen aan een bericht. Zie [limieten voor journaal, vervoer, en postvak in](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)voor meer informatie.
    
- Regels van postvak in werken op het postvak van de andere berichten niet. Zie voor meer informatie over de postbus alternatieve logboekregistratie [postbus alternatieve logboekregistratie in](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
U kunt deze problemen oplossen door Zie [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Als de bovenstaande problemen zijn niet van toepassing, het postvak in regel diagnostisch rapport uitvoeren voordat u het probleem aan Microsoft Support escaleren:
  
1. Open het postvak in Outlook op het web en klik op **Instellingen** \> **Opties** \> **e-mail organiseren** \> **regels voor postvak in**.
    
2. Klik onderaan de pagina op **Als uw regels niet, klikt u hier werkt voor het genereren van een diagnostisch rapport**.
    

