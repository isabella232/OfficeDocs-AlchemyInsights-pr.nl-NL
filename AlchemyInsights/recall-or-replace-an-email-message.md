---
title: Een e-mailbericht intrekken of vervangen
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
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742750"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Een e-mailbericht in Microsoft 365 intrekken of vervangen

- U **alleen berichten terugroepen die naar mensen in uw organisatie worden verzonden.** Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, u het niet meer herinneren.
- U **alleen berichten terugroepen die vanuit Outlook 2016 voor de pc zijn verzonden.** Als een gebruiker een bericht verzendt met de webversie van Outlook voor Mac of Outlook, u dit niet meer herinneren.
- Als u een beheerder bent, u **berichten namens gebruikers terugroepen met PowerShell.** U berichten van het beheercentrum niet meer in herinnering roepen. Scroll naar beneden naar 'E-mailberichten zoeken en verwijderen in uw organisatie' voor meer informatie.

**Een e-mailbericht terugroepen of vervangen dat u hebt verzonden**

1. Kies in het mappenvenster links van het Outlook-venster de map Verzonden items.
2. Open het bericht dat u wilt herinneren. U moet dubbelklikken om het bericht te openen. Als u het bericht selecteert zodat het in het leesvenster wordt weergegeven, u het bericht niet inherinnering roepen.
3. Selecteer op het tabblad Bericht de optie **Acties** > **Dit bericht terugroepen**.
4. Kies **Ongelezen exemplaren van dit bericht verwijderen** of **Ongelezen exemplaren verwijderen en vervangen door een nieuw bericht**en selecteer **OK**.
5. Als u een vervangend bericht verzendt, stelt u het bericht samen en selecteert u **Verzenden**.
6. Het succes of het mislukken van een berichtterugroeping is afhankelijk van de instellingen van de geadresseerden in Outlook.

Zie [Een e-mailbericht dat u](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)hebt verzonden voor meer informatie, inclusief hoe u de terugroepactie controleren.

***E-mailberichten in uw organisatie zoeken en verwijderen*** Als u e-mailberichten in uw organisatie wilt zoeken en verwijderen, is het het gemakkelijkst als u een globale beheerder bent. Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rolgroep eDiscovery Manager of aan de rol Van Het Zoeken naar naleving. Als u berichten wilt verwijderen, moet u lid worden van de rolgroep Organisatiebeheer of de rol Zoek- en Zuiveringsbeheer. Machtigingen voor deze rollen worden toegewezen in het [beveiligingscentrum &.](https://protection.office.com/)

1. [Maak een inhoudszoekopdracht](https://docs.microsoft.com/office365/securitycompliance/content-search) om het bericht te vinden dat moet worden verwijderd.
2. [Maak verbinding met Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Zie Verbinding maken met [Microsoft 365-beveiliging & Compliance Center PowerShell met behulp van multi-factor authenticatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)als u MFA gebruikt. 
