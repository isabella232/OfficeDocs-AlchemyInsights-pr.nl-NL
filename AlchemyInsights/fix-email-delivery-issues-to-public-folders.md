---
title: Problemen met e-mailbezorging oplossen in openbare mappen met e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716347"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Problemen met e-mailbezorging oplossen in openbare mappen met e-mail

Als externe afzenders geen berichten naar uw openbare mappen met e-mail kunnen verzenden en de afzenders de fout ontvangen: **kan niet worden gevonden (550 5.4.1),** controleert u of het e-maildomein voor de openbare map is geconfigureerd als een intern relaydomein in plaats van een gezaghebbend domein:

1. Open het [Exchange-beheercentrum (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Ga naar **Geaccepteerde domeinen** **e-mail,** \> selecteer het geaccepteerde domein en klik op **Bewerken**.

3. Als het domeintype op de pagina eigenschappen wordt geopend, **wijzigt**u de waarde in **Intern relay** en klikt u op **Opslaan**.

Als externe afzenders de fout ontvangen **die u niet hebt (550 5.7.13),** voert u de volgende opdracht uit in Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) om de machtigingen voor anonieme gebruikers in de openbare map te bekijken:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Bijvoorbeeld. `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

Als u externe gebruikers wilt toestaan e-mail naar deze openbare map te verzenden, voegt u het toegangsrecht voor Items maken toe aan de gebruiker Anoniem. Bijvoorbeeld `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
