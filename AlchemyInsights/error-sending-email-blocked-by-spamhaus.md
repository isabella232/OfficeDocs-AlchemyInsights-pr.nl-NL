---
title: Fout bij verzenden e-mail geblokkeerd door SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783798"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fout bij verzenden e-mail: client host geblokkeerd met behulp van Spamhaus

Het IP-adres dat het bericht heeft verstuurd bevindt zich op een bloklijst met de eigenaar van [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Redenen om te worden geblokkeerd door Spamhaus zijn in gebruik zijnde accounts, het delen van een openbaar IP-adres en een beleidsregels voor internetproviders. Mogelijke oplossingen zijn:
  
- Voor geblokkeerde inkomende berichten waarop u de bron-e-mailserver beheert, dient u de oorzaak vast te stellen en de blokkering van de Spamhaus-website te verwijderen.

- Voor geblokkeerde inkomende berichten waarvan het bron-IP-adres lid is van iemand anders, moet de adres eigenaar de blokkering van de Spamhaus-website verwijderen. Als het IP-adres zich in de lijst met beleids blokkering (PBL) bevindt, kan de eigenaar een ander statisch IP-adres toewijzen of het adres verwijderen uit de PBL.

- Voor geblokkeerde uitgaande berichten van uw domein verbonden met Microsoft, kunt u deze fout weergegeven als de berichten worden gerouteerd via een service van een andere leverancier. U kunt een WHOIS-zoekprogramma gebruiken om de geblokkeerde IP-adres eigenaar te vinden.
