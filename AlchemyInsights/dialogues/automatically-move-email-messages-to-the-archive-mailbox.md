---
title: E-mailberichten automatisch naar het archiefpostvak verplaatsen
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525094"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>E-mailberichten automatisch naar het archiefpostvak verplaatsen

U kunt als volgende manier een beleid instellen om oude e-mailberichten van een gebruiker automatisch naar het archiefpostvak te verplaatsen:

1. Ga naar [**het & compliancegegevensbeheerarchief**](https://go.microsoft.com/fwlink/p/?linkid=2077143)om te controleren of een archiefpostvak is ingeschakeld  >    >   voor de gebruiker. Als dat niet zo is, klikt u **in** **het waarschuwingsvak** op Inschakelen en Ja.
2. Ga naar [**het Exchange-beheercentrum voor > compliancebeheer > bewaarlabels.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Kies het pictogram + en kies vervolgens **automatisch toepassen op het hele postvak.**
4. Wijs een naam toe aan de bewaartag en kies **Verplaatsen naar archief.** Voer voor de bewaarperiode de beste tijd in, bijvoorbeeld 90 dagen. Klik op **Opslaan**.
5. Maak nu een bewaarbeleid: kies **bewaarbeleid en** kies het pictogram om een nieuw beleid toe te voegen.
6. Wijs een naam toe aan het bewaarbeleid en klik en schuif om de bewaartag die u zojuist hebt gemaakt te zoeken en toe te voegen. Klik op **Opslaan**.
7. Ten slotte past u het bewaarbeleid toe op het postvak van de gebruiker: ga nog steeds in het Exchange-beheercentrum naar de postvakken  >  **van geadresseerden.** Kies alle gebruikers op wie u het beleid wilt toepassen en kies vervolgens **Bewerken** (het potloodpictogram).
8. Klik in het dialoogvenster op **postvakfuncties.** Pas **onder Bewaarbeleid** het beleid toe dat u zojuist hebt gemaakt > **Opslaan.**
9. Zie Een bewaarbeleid toepassen op postvakken voor instructies voor het toepassen van het beleid [op alle gebruikers.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
