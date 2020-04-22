---
title: Fout verzenden e-mail geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714253"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fout verzenden e-mail: Clienthost geblokkeerd met Spamhaus

Het IP-adres dat het bericht heeft verzonden, staat op een bloklijst die eigendom is van [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Redenen om geblokkeerd te worden door Spamhaus zijn gecompromitteerde accounts, gecompromitteerde machines die een openbaar IP-adres delen en internetserviceprovider (ISP)-beleid. Mogelijke oplossingen zijn:
  
- Voor geblokkeerde binnenkomende berichten waarin u de brone-mailserver beheert, moet u de oorzaak bepalen en het blok verwijderen van de Spamhaus-website.

- Voor geblokkeerde binnenkomende berichten waarbij het ip-adres van de bron van iemand anders is, moet de adreseigenaar het blok verwijderen van de Spamhaus-website. Als het IP-adres op de Beleidsbloklijst (PBL) staat, kan de eigenaar een ander statisch IP-adres toewijzen of het adres van het PBL verwijderen.

- Voor geblokkeerde uitgaande berichten uit uw domein die zijn verbonden met Microsoft, u deze fout ontvangen als de berichten worden doorgestuurd via een service van derden. U een WHOIS-opzoektool gebruiken om de eigenaar van het geblokkeerde IP-adres te vinden.
