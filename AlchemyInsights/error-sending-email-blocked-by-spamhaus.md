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
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946709"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fout bij het verzenden van e-mail: Clienthost geblokkeerd met Spamhaus

Het IP-adres dat het bericht heeft verzonden, staat in een bloklijst die eigendom is van [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Redenen voor het blokkeren door Spamhaus zijn gecompromitteerde accounts, gecompromitteerde computers die een openbaar IP-adres delen en internetproviderbeleid. Mogelijke oplossingen zijn:
  
- Voor geblokkeerde binnenkomende berichten waarin u de bron-e-mailserver controleert, moet u de oorzaak bepalen en het blok verwijderen van de spamhaus-website.

- Voor geblokkeerde binnenkomende berichten waarbij het bron-IP-adres van iemand anders is, moet de eigenaar van het adres het blok van de spamhaus-website verwijderen. Als het IP-adres zich in de lijst met beleidsblokkeringen (PBL) vindt, kan de eigenaar een ander statisch IP-adres toewijzen of het adres uit het PBL verwijderen.

- Voor geblokkeerde uitgaande berichten van uw domein die zijn verbonden met Microsoft, kunt u deze fout ontvangen als de berichten worden gerouteerd via een service van derden. U kunt een WHOIS-zoekprogramma gebruiken om de geblokkeerde eigenaar van het IP-adres te zoeken.
