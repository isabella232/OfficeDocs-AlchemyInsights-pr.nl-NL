---
title: Een e-mailbericht intrekken of vervangen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353501"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Een e-mailbericht intrekken of vervangen in Microsoft 365

- U kunt **alleen berichten intrekken die zijn verzonden naar personen in uw organisatie**. Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kunt u dit niet intrekken.
- U kunt **alleen berichten intrekken die vanuit Outlook voor de PC zijn verzonden**. Als een gebruiker een bericht verzendt met Outlook voor Mac of de webversie van Outlook, kunt u dit niet intrekken.
- Als tenantbeheerder kunt u **berichten intrekken namens gebruikers met behulp van PowerShell** (Zie [e-mailberichten zoeken en verwijderen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)voor meer informatie.)
- U kunt geen berichten intrekken vanuit het Beheercentrum. Schuif omlaag naar e-mailberichten in uw organisatie zoeken en verwijderen voor meer informatie.

**Een verzonden e-mailbericht intrekken of vervangen**

1. Kies in het mappenvenster links van het Outlook-venster de map Verzonden items.
2. Open het bericht dat u wilt intrekken. U dubbelklikt op het bericht om het te openen. Als u het bericht selecteert zodat het in het leesvenster wordt weergegeven, kunt u het bericht niet meer intrekken.
3. Selecteer op het tabblad bericht de optie **acties**  >  **Dit bericht intrekken**.
4. Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht** en klik vervolgens op **OK**.
5. Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u vervolgens **verzenden**.
6. Het slagen of mislukken van het intrekken van een bericht is afhankelijk van de instellingen van de ontvangers in Outlook.

Zie [een verzonden e-mailbericht intrekken of vervangen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor meer informatie, waaronder het intrekken van een bericht.

Als u **_e-mailberichten in uw organisatie wilt zoeken en verwijderen_**, kunt u dit het beste doen als u een globale beheerder bent. Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rollen groep van de eDiscovery-beheerder of aan de rol zoekbeheer voor naleving. Als u berichten wilt verwijderen, moet u lid worden van de rollen groep Organisatiebeheer of de rol zoeken en wissen. Machtigingen voor deze rollen worden toegewezen in de [beveiligings & nalevings centrum](https://protection.office.com/).

1. [Maak een zoekopdracht naar inhoud](https://docs.microsoft.com/microsoft-365/compliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.
2. [Maak verbinding met beveiliging & nalevings centrum voor PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Zie [verbinding maken met Microsoft 365-beveiliging & nalevings centrum voor PowerShell via meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)als u MFA gebruikt (multi-factor Authentication).
