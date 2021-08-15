---
title: Een e-mailbericht in- of vervangen
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024381"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Een e-mailbericht in- of Microsoft 365

- U kunt **alleen berichten inroepen die naar personen in uw organisatie zijn verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kunt u het niet meer terugroepen.
- U kunt **alleen berichten inroepen die zijn verzonden Outlook voor de pc.** Als een gebruiker een bericht verzendt met Outlook voor Mac of webversie van Outlook, kunt u het bericht niet meer terughalen.
- Als tenantbeheerder kunt u berichten namens gebruikers inroepen met Behulp van **PowerShell** (Zie Voor meer informatie: E-mailberichten zoeken en [verwijderen).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- U kunt geen berichten uit het beheercentrum inroepen. Schuif omlaag naar 'E-mailberichten zoeken en verwijderen in uw organisatie' voor meer informatie.

**Een e-mailbericht dat u hebt verzonden in- of vervangen**

1. Kies in het mappenvenster aan de linkerkant van Outlook venster de map Verzonden items.
2. Open het bericht dat u wilt inroepen. U moet dubbelklikken om het bericht te openen. Als u het bericht selecteert zodat het wordt weergegeven in het leesvenster, kunt u het bericht niet inroepen.
3. Selecteer op het tabblad Bericht **de optie Acties**  >  **Inroepen van dit bericht.**
4. Kies **Ongelezen exemplaren van** dit bericht verwijderen of **Ongelezen** exemplaren verwijderen en vervangen door een nieuw bericht en selecteer **OK.**
5. Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u **Vervolgens Verzenden**.
6. Het succes of de fout van een bericht inroepen is afhankelijk van de instellingen van de geadresseerden in Outlook.

Zie Een e-mailbericht dat u hebt verzonden in- of vervangen voor meer informatie, waaronder hoe u het inroepen [kunt controleren.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Als u e-mailberichten in*** uw organisatie wilt zoeken en verwijderen, is het het gemakkelijkst als u een globale beheerder bent. Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rollengroep eDiscovery Manager of aan de beheerrol Compliance search. Als u berichten wilt verwijderen, moet u lid worden van de rollengroep Organisatiebeheer of de rol zoeken en verwijderen. Machtigingen voor deze rollen worden toegewezen in het beveiligings- [& compliancecentrum.](https://protection.office.com/)

1. [Maak een inhoudszoekactie](https://docs.microsoft.com/microsoft-365/compliance/content-search) om het bericht te vinden dat u wilt verwijderen.
2. [Verbinding maken met Beveiligings- en compliancecentrum van Powershell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Als u MFA (meervoudige verificatie) gebruikt, kunt u Verbinding maken Microsoft 365 [Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)gebruiken met meervoudige verificatie.
