---
title: E-mail levering problemen oplossen naar e-mailadres van openbare mappen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401323"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-mail levering problemen oplossen naar e-mailadres van openbare mappen

Externe afzenders geen berichten verzenden naar uw e-mailadres openbare mappen als de afzenders, wordt het foutbericht: **(550 5.4.1) niet is gevonden**, controleert u of het e-maildomein voor de openbare map is geconfigureerd als een intern relay-domein in plaats van een gezaghebbende domein:

1. Open het [beheercentrum van Exchange (SBV)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Ga naar de **e-mailstroom** \> **geaccepteerde domeinen**, selecteert u het geaccepteerde domein en klik vervolgens op **bewerken**.

3. In de eigenschappen pagina die wordt geopend als het domeintype **bindend**, wijzig de waarde in **interne relay** en klik op **Opslaan**.

Als externe afzenders ontvangt de fout- **u hebt geen machtiging (550 5.7.13)**, moet u de volgende opdracht uitvoeren in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) om te zien welke machtigingen voor anonieme gebruikers in de openbare map:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Bijvoorbeeld `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Zodat externe gebruikers e-mail verzenden naar deze openbare map toevoegen de CreateItems toegang aan de gebruiker anoniem. Bijvoorbeeld `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
