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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744850"
---
# <a name="fix-connection-policy"></a>Verbindingsbeleid oplossen

De e-mail is als veilig gemarkeerd en bezorgd in het Postvak IN van de gebruiker omdat het verzendende IP-adres veilig is gemarkeerd in het beleid voor verbindingsfilter. Ga als volgt te werk om het beleid te bekijken:

1. Ga naar het [Office 365-beveiligings- & compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga vervolgens naar **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Selecteer op **het** tabblad Aangepast het **verbindingsfilterbeleid** en selecteer **vervolgens Beleid bewerken.**
3. Bekijk de **lijst IP-toestaan.** Kijk of **Lijst met veilige** gebruikers is ingeschakeld.

    > [!NOTE]
    > Microsoft is geabonneerd op externe bronnen van vertrouwde afzenders. Als **De lijst Veilig** is ingeschakeld, worden deze vertrouwde afzenders niet per ongeluk gemarkeerd als spam. Ik raad u aan deze optie te selecteren, omdat hiermee het aantal fout-positieven (goede e-mail die als spam is geclassificeerd) wordt beperkt.
