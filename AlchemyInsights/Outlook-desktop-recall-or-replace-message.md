---
title: Outlook Desktop terugroepen of vervangen van een e-mail bericht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496106"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Een Outlook-e-mail bericht intrekken of vervangen

- Als beheerder u **berichten intrekken namens gebruikers die PowerShell gebruiken**. U geen berichten terughalen uit het Admin Center.
- U **alleen berichten terughalen die worden verzonden naar mensen in uw organisatie**. Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, u het niet meer terughalen.
- U **alleen berichten terughalen die vanuit Outlook 2016 op de PC zijn verzonden**. Als een gebruiker een bericht verzendt met Outlook voor Mac of Outlook op het web, u het niet meer intrekken.

Een e-mail bericht intrekken of vervangen:

1. Selecteer in het mappenvenster aan de linkerkant van het Outlook-venster de map Verzonden items.
1. Dubbelklik op het bericht dat u wilt intrekken om het te openen.
1. Selecteer het tabblad **bericht** en selecteer vervolgens **acties** > **intrekken dit bericht**.
1. Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht**en selecteer vervolgens **OK**.
1. Als u een vervangend bericht verzendt, moet u het bericht opstellen en vervolgens **verzenden**selecteren.
1. Het slagen of mislukken van een bericht intrekken is afhankelijk van de instellingen van de geadresseerde in Outlook. Zie [dit artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor stappen om te controleren op de terugroepactie.

E-mail berichten in uw organisatie zoeken en verwijderen

- Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol van eDiscovery Manager of beheer van naleving zoeken om te zoeken naar berichten. Als u wilt verwijderen van berichten, moet u deelnemen aan de organisatiemanagement rol groep of de Search and purge Management rol. Machtigingen voor deze rollen worden toegewezen in het [beveiligings-en compliancecentrum](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Maak een zoekopdracht voor inhoud](https://docs.microsoft.com/office365/securitycompliance/content-search) om het bericht te zoeken dat u wilt verwijderen.
- [Verbinding maken met Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Als u multi-factor Authentication gebruikt, Zie [verbinding maken met Office 365 Security and Compliance Center PowerShell met behulp van meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).