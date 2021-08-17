---
title: Verbindingsbeleid oplossen
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888401"
---
# <a name="fix-connection-policy"></a>Verbindingsbeleid oplossen

De e-mail is als veilig gemarkeerd en bezorgd in het Postvak IN van de gebruiker omdat het bron-IP-adres is gemarkeerd als veilig in het standaardbeleid voor verbindingsfilters. Als u het beleid wilt controleren, gaat u als volgt te werk:

1. Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com/> **E-mail & Samenwerkingsbeleid** & Beleidsregels voor bedreigingsregels \>  \>  \> **Antispam** in  de sectie Beleid.

   Gebruik <https://security.microsoft.com/antispam> om direct naar de pagina **Antispambeleid** te gaan.

2. Selecteer op **de pagina Antispambeleid** het beleid met de naam **Verbindingsfilterbeleid (standaard)** door op de naam van het beleid te klikken.

3. Klik in de flyout details die wordt weergegeven op **Verbindingsfilterbeleid bewerken** in **de sectie Verbindingsfilter.**

4. Controleer de vermeldingen in de sectie Altijd toestaan berichten uit de volgende **sectie IP-adressen** of adresbereik en kijk of **Veilige** lijst in-/uit-lijst in- of uit- of uit te stellen is geselecteerd.

   > [!NOTE]
   > Microsoft is geabonneerd op externe bronnen van vertrouwde afzenders. Als de veilige lijst is ingeschakeld, worden deze vertrouwde afzenders niet per ongeluk gemarkeerd als spam. U wordt aangeraden deze optie te selecteren, omdat hierdoor het aantal onwaar-positieven (goede e-mail die als spam is geclassificeerd) wordt beperkt.

Zie [Verbindingsfiltering configureren](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy) voor meer informatie.
