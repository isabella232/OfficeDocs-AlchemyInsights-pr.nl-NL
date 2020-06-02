---
title: Outlook Desktop herinnert of vervangt een e-mailbericht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502314"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Een Outlook-e-mailbericht intrekken of vervangen

- Als beheerder u **berichten namens gebruikers intrekken met PowerShell.** U berichten van het beheercentrum niet meer herinneren.
- U **alleen berichten terugroepen die naar mensen in uw organisatie worden verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kun je het niet meer herinneren.
- U **alleen berichten die vanuit Outlook 2016 op de pc zijn verzonden, terugroepen.** Als een gebruiker een bericht verzendt met Outlook voor Mac of Outlook in de webversie, u het zich niet herinneren.

Een e-mailbericht intrekken of vervangen:

1. Selecteer in het mappenvenster aan de linkerkant van het Outlook-venster de map Verzonden items.
1. Dubbelklik op het bericht dat u wilt inroepen om het bericht te openen.
1. Selecteer het tabblad **Bericht** en selecteer **Acties**  >  **Dit bericht terugroepen**.
1. Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht**en selecteer **Vervolgens OK**.
1. Als u een vervangend bericht verzendt, stelt u het bericht samen en selecteert u **Verzenden**.
1. Het succes of het mislukken van een berichtherinnering is afhankelijk van de instellingen van de ontvanger in Outlook. Zie [dit artikel voor](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)stappen om de terugroepactie te controleren.

E-mailberichten zoeken en verwijderen in uw organisatie

- Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol eDiscovery Manager of de rol Voor het beheer van compliancezoekopdrachten om naar berichten te zoeken. Als u berichten wilt verwijderen, moet u lid worden van de rolgroep Organisatiebeheer of de beheerrol Zoeken en zuiveren. Machtigingen voor deze rollen worden toegewezen in het [beveiligings- en compliancecentrum](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Maak een inhoudszoekopdracht](https://docs.microsoft.com/microsoft-365/compliance/content-search) om het bericht te vinden dat moet worden verwijderd.
- [Maak verbinding met PowerShell van beveiligings- en compliancecentrum.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Zie Verbinding maken met [Microsoft 365-beveiligings- en Compliance Center PowerShell met behulp van meervoudige verificatie als](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)u meerstapsverificatie gebruikt.