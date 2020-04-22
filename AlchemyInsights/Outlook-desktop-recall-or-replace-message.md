---
title: Een e-mailbericht terugroepen of vervangen door Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687505"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Een Outlook-e-mailbericht intrekken of vervangen

- Als beheerder u **berichten terugroepen namens gebruikers die PowerShell gebruiken.** U berichten van het beheercentrum niet meer in herinnering roepen.
- U **alleen berichten terugroepen die naar mensen in uw organisatie worden verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, u het niet meer herinneren.
- U **alleen berichten terugroepen die vanuit Outlook 2016 op de pc zijn verzonden.** Als een gebruiker een bericht verzendt met de webversie van Outlook voor Mac of Outlook, u dit niet meer herinneren.

Een e-mailbericht terugroepen of vervangen:

1. Selecteer in het mappenvenster links van het Outlook-venster de map Verzonden items.
1. Dubbelklik op het bericht dat u wilt inroepen om het te openen.
1. Selecteer het tabblad **Bericht** en selecteer **Vervolgens Acties** > **Dit bericht terugroepen**.
1. Selecteer **Ongelezen exemplaren van dit bericht verwijderen** of **Ongelezen exemplaren verwijderen en vervangen door een nieuw bericht**en selecteer **OK**.
1. Als u een vervangend bericht verzendt, stelt u het bericht samen en selecteert u **Verzenden**.
1. Het succes of het mislukken van een berichtterugroeping is afhankelijk van de instellingen van de ontvanger in Outlook. Zie [dit artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor stappen om de terugroepactie te controleren.

E-mailberichten in uw organisatie zoeken en verwijderen

- Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol eDiscovery Manager of de rol Compliance Search-beheer om naar berichten te zoeken. Als u berichten wilt verwijderen, moet u lid worden van de rolgroep Organisatiebeheer of de rol Zoek- en Zuiveringsbeheer. Machtigingen voor deze rollen worden toegewezen in het [beveiligings- en compliancecentrum](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Maak een inhoudszoekopdracht](https://docs.microsoft.com/office365/securitycompliance/content-search) om het bericht te vinden dat moet worden verwijderd.
- [Maak verbinding met Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Zie [Verbinding maken met Microsoft 365 security en Compliance Center PowerShell met multi-factor authenticatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)als u multi-factor authenticatie gebruikt.