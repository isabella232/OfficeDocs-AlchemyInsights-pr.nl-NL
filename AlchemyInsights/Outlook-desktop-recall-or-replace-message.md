---
title: Outlook Een e-mailbericht in- of vervangen
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918390"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Een e-mailbericht in- of Outlook in- of vervangen

- Als beheerder kunt u berichten **inroepen namens gebruikers die PowerShell gebruiken.** U kunt geen berichten uit het beheercentrum inroepen.
- U kunt **alleen berichten inroepen die naar personen in uw organisatie zijn verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kunt u het niet meer terugroepen.
- U kunt **alleen berichten inroepen die zijn verzonden Outlook 2016 op de pc.** Als een gebruiker een bericht verzendt met Outlook voor Mac of webversie van Outlook, kunt u het bericht niet meer terughalen.

Een e-mailbericht in- of vervangen:

1. Selecteer in het mappenvenster aan de linkerkant van Outlook venster de map Verzonden items.
1. Dubbelklik op het bericht dat u wilt inroepen om het te openen.
1. Selecteer het **tabblad** Bericht en selecteer vervolgens **Acties Dit** bericht  >  **inroepen.**
1. Selecteer **Ongelezen kopieën van dit bericht verwijderen of** **Ongelezen** kopieën verwijderen en vervangen door een nieuw bericht en selecteer **OK.**
1. Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u **Vervolgens Verzenden**.
1. Het succes of de fout van een bericht inroepen is afhankelijk van de instellingen van de geadresseerde in Outlook. Zie dit artikel voor stappen om het inroepen [te controleren.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

E-mailberichten in uw organisatie zoeken en verwijderen

- Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol eDiscovery Manager of de rol van compliancezoekbeheer om berichten te zoeken. Als u berichten wilt verwijderen, moet u lid worden van de rollengroep Organisatiebeheer of de rol zoeken en verwijderen. Machtigingen voor deze rollen worden toegewezen in het [beveiligings- en compliancecentrum.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Maak een inhoudszoekactie](https://docs.microsoft.com/microsoft-365/compliance/content-search) om het bericht te vinden dat u wilt verwijderen.
- [Verbinding maken beveiligings- en compliancecentrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Als u meervoudige verificatie gebruikt, bekijkt u Verbinding maken voor Microsoft 365 en Compliance center PowerShell met [meervoudige verificatie.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)