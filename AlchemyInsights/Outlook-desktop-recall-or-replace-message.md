---
title: Een e-mailbericht intrekken of vervangen in de bureaubladversie van Outlook
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663985"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Een e-mailbericht intrekken of vervangen in Outlook

- Als beheerder kunt u **berichten intrekken namens gebruikers met behulp van PowerShell**. U kunt geen berichten intrekken vanuit het Beheercentrum.
- U kunt **alleen berichten intrekken die zijn verzonden naar personen in uw organisatie**. Als het bericht is verzonden naar een Gmail-adres, kunt u dit bijvoorbeeld niet intrekken.
- U kunt **alleen berichten intrekken die vanuit Outlook 2016 op de PC zijn verzonden**. Als een gebruiker een bericht verzendt met Outlook voor Mac of de webversie van Outlook, kunt u dit niet intrekken.

Een e-mailbericht intrekken of vervangen:

1. Selecteer in het deelvenster map aan de linkerkant van het Outlook-venster de map Verzonden items.
1. Dubbelklik op het bericht dat u wilt intrekken om het te openen.
1. Selecteer het tabblad **bericht** en selecteer vervolgens **actie**  >  **Dit bericht intrekken**.
1. Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht**en klik vervolgens op **OK**.
1. Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u vervolgens **verzenden**.
1. Het slagen of mislukken van het intrekken van een bericht is afhankelijk van de instellingen van de geadresseerde in Outlook. Zie het [volgende artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor de stappen voor het intrekken van een bericht.

E-mailberichten in uw organisatie zoeken en verwijderen

- Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol van eDiscovery-beheerder of zoekbeheer voor compliance om te zoeken naar berichten. Als u berichten wilt verwijderen, moet u lid worden van de rollen groep Organisatiebeheer of de rol zoeken en wissen. Machtigingen voor deze rollen worden toegewezen in het [beveiligings-en compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Maak een zoekopdracht naar inhoud](https://docs.microsoft.com/microsoft-365/compliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.
- [Maak verbinding met het beveiligings-en compliance-centrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Als u multi-factor Authentication gebruikt, raadpleegt u [verbinding maken met de PowerShell-beveiliging en compliance van Microsoft 365 via meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).