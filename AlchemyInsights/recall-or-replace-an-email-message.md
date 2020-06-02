---
title: Een e-mailbericht terugroepen of vervangen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509451"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Een e-mailbericht intrekken of vervangen in Microsoft 365

- U **alleen berichten terugroepen die naar mensen in uw organisatie worden verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kun je het niet meer herinneren.
- U **alleen berichten inroepen die zijn verzonden vanuit Outlook 2016 voor de pc**. Als een gebruiker een bericht verzendt met Outlook voor Mac of Outlook in de webversie, u het zich niet herinneren.
- Als u een beheerder bent, u **berichten namens gebruikers intrekken met Behulp van PowerShell**. U berichten van het beheercentrum niet meer herinneren. Blader omlaag naar 'E-mailberichten zoeken en verwijderen in uw organisatie' voor meer informatie.

**Een e-mailbericht dat u hebt verzonden, in- of vervang**

1. Kies in het mappenvenster aan de linkerkant van het Outlook-venster de map Verzonden items.
2. Open het bericht dat u wilt inroepen. U moet dubbelklikken om het bericht te openen. Als u het bericht zo selecteert dat het in het leesvenster wordt weergegeven, u het bericht niet terugroepen.
3. Selecteer op het tabblad Bericht de optie **Acties**  >  **dit bericht terugroepen**.
4. Kies **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervang door een nieuw bericht**en selecteer **vervolgens OK**.
5. Als u een vervangend bericht verzendt, stelt u het bericht samen en selecteert u **Verzenden**.
6. Het succes of het mislukken van een berichtherinnering is afhankelijk van de instellingen van de geadresseerden in Outlook.

Zie [Een e-mailbericht dat u hebt verzonden voor](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)meer informatie, zoals hoe u de terugroepactie controleren.

***E-mailberichten zoeken en verwijderen in uw organisatie*** Als u e-mailberichten in uw organisatie wilt zoeken en verwijderen, is het het gemakkelijkst als u een globale beheerder bent. Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rolgroep eDiscovery Manager of aan de rol van Compliance Search Management. Als u berichten wilt verwijderen, moet u lid worden van de rolgroep Organisatiebeheer of de beheerrol Zoeken en zuiveren. Machtigingen voor deze rollen worden toegewezen in het [security & compliance center](https://protection.office.com/).

1. [Maak een inhoudszoekopdracht](https://docs.microsoft.com/microsoft-365/compliance/content-search) om het bericht te vinden dat moet worden verwijderd.
2. [Maak verbinding met PowerShell & Security-&.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

Zie Verbinding maken met [Microsoft 365-beveiligingscentrum & PowerShell met behulp van meervoudige verificatie als](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)u MFA gebruikt. 
