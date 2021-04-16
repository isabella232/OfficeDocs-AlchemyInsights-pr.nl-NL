---
title: Fout bij het verzenden van e-mail die is geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813719"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fout bij het verzenden van e-mail: Clienthost geblokkeerd met Spamhaus

Het IP-adres dat het bericht heeft verzonden, staat in een bloklijst die eigendom is van [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Redenen voor het blokkeren door Spamhaus zijn gecompromitteerde accounts, gecompromitteerde computers die een openbaar IP-adres delen en internetproviderbeleid. Mogelijke oplossingen zijn:
  
- Voor geblokkeerde binnenkomende berichten waarin u de bron-e-mailserver controleert, moet u de oorzaak bepalen en het blok verwijderen van de spamhaus-website.

- Voor geblokkeerde binnenkomende berichten waarbij het bron-IP-adres van iemand anders is, moet de eigenaar van het adres het blok van de spamhaus-website verwijderen. Als het IP-adres zich in de lijst met beleidsblokkeringen (PBL) vindt, kan de eigenaar een ander statisch IP-adres toewijzen of het adres uit het PBL verwijderen.

- Voor geblokkeerde uitgaande berichten van uw domein die zijn verbonden met Microsoft, kunt u deze fout ontvangen als de berichten worden gerouteerd via een service van derden. U kunt een WHOIS-zoekprogramma gebruiken om de geblokkeerde eigenaar van het IP-adres te zoeken.
