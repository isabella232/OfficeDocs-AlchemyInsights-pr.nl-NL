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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988086"
---
# <a name="fix-connection-policy"></a>Verbindingsbeleid oplossen

De e-mail is als veilig gemarkeerd en bezorgd in het Postvak IN van de gebruiker omdat het verzendende IP-adres veilig is gemarkeerd in het beleid voor verbindingsfilter. Ga als volgt te werk om het beleid te bekijken:

1. Ga naar het [Office 365 beveiligingscentrum & compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga naar **Beleid** voor  >    >  [bedreigingsbeheer antispam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Selecteer op **het** tabblad Aangepast het **verbindingsfilterbeleid** en selecteer **vervolgens Beleid bewerken.**
3. Bekijk de **lijst IP-toestaan.** Kijk of **Safe is** ingeschakeld.

    > [!NOTE]
    > Microsoft is geabonneerd op externe bronnen van vertrouwde afzenders. Als **Safe is** ingeschakeld, worden deze vertrouwde afzenders niet per ongeluk gemarkeerd als spam. Ik raad u aan deze optie te selecteren, omdat hiermee het aantal fout-positieven (goede e-mail die als spam is geclassificeerd) wordt beperkt.
