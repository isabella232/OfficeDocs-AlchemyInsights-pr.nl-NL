---
title: Fout bij het verzenden van e-mailadres is geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912343"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fout bij het verzenden van e-mail: Client host is geblokkeerd met behulp van Spamhaus

Het IP-adres voor het bericht is op een lijst met geblokkeerde websites die eigendom zijn van [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Redenen voor zijn geblokkeerd in de Spamhaus zijn gekraakte accounts, machines, delen van een openbaar IP-adres en een Internet Service Provider (ISP) beleid in gevaar gebracht. Mogelijke oplossingen zijn:
  
- Voor binnenkomende berichten geblokkeerd voor Office 365, waar u de bron-e-mailserver beheren, moet u de oorzaak en het blok verwijderen vanaf de website van Spamhaus.
    
- Voor binnenkomende berichten geblokkeerd met Office 365 waar het bron-IP-adres van iemand anders, moet de eigenaar van het adres het blok verwijderen vanaf de website van Spamhaus. Als het IP-adres op het beleid blokkeren lijst (PBL), kan de eigenaar een andere statische IP-adres toewijzen of verwijderen van het adres van de PBL.
    
- Voor uitgaande berichten uit uw domein van Office 365 geblokkeerd, kunt u deze fout optreden als de berichten worden gerouteerd via een 3e partij. Een WHOIS lookup tool kunt u de eigenaar van de geblokkeerde IP-adres vinden.
    

