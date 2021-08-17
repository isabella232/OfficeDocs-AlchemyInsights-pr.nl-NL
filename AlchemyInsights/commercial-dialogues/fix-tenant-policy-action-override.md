---
title: Tenantbeleid oplossen (actie overschrijven)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896070"
---
# <a name="fix-tenant-policy-action-override"></a>Tenantbeleid oplossen (actie overschrijven)

Een van uw antispambeleid heeft dit bericht beïnvloed. Als u het beleid wilt controleren, gaat u als volgt te werk:

1. Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com/> **E-mail & Samenwerkingsbeleid** & Beleidsregels voor bedreigingsregels \>  \>  \> **Antispam** in  de sectie Beleid.

   Gebruik <https://security.microsoft.com/antispam> om direct naar de pagina **Antispambeleid** te gaan.

2. Selecteer op de pagina Antispambeleid het beleid door op de naam van het beleid te klikken (**Type** is Aangepast **antispambeleid** of Naam **is** **antispam binnenkomende beleid (standaard)**). 
3. Selecteer in het detail flyout dat wordt weergegeven de optie **Acties bewerken** in de **sectie** Acties.
4. Bekijk in **de sectie Berichtacties** de vonnissen voor **Spam,** Spam met hoog **vertrouwen,** **Phishing** en **phishing** met hoog vertrouwen om te zien of een van de volgende waarden is geselecteerd:
   - **X-header toevoegen**
   - **Onderwerpregel voorbereiden met tekst**
   - **Bericht omleiden naar e-mailadres**
   - **Bericht verwijderen**
   - **Geen actie**

   Het is mogelijk dat de standaardinstellingen **die** zijn toegepast op alle Exchange Online Protection het bericht hebben beïnvloed.

Zie [Antispambeleid configureren in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies) voor meer informatie.
