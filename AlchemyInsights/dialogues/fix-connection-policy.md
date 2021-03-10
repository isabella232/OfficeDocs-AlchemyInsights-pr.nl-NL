---
title: Verbindingsbeleid herstellen
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693301"
---
# <a name="fix-connection-policy"></a>Verbindingsbeleid herstellen

Het e-mailbericht is als veilig gemarkeerd en bezorgd in het Postvak IN van de gebruiker omdat het verzendende IP-adres als veilig is gemarkeerd in het verbindingsfilterbeleid. Ga als volgt te werk om het beleid te controleren:

1. Ga naar het [Office 365-& compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga naar Beleid voor bedreigingsbeheer  >    >  [antispam.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Selecteer op **het tabblad** Aangepast het **verbindingsfilterbeleid** en selecteer beleid **bewerken.**
3. Bekijk de lijst **met toegestane IP-adressen.** Kijk of **De lijst** Veilig is ingeschakeld.

    > [!NOTE]
    > Microsoft abonneert zich op bronnen van vertrouwde afzenders van derden. Als **de lijst** Veilig is ingeschakeld, worden deze vertrouwde afzenders niet per ongeluk gemarkeerd als spam. Het is raadzaam deze optie te selecteren, omdat hiermee het aantal fout-positieven (goede e-mail die als spam is geclassificeerd) wordt beperkt.
