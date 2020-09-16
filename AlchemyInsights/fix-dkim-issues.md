---
title: Problemen met de installatie van DKIM oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744945"
---
# <a name="fix-dkim-setup-issues"></a>Problemen met de installatie van DKIM oplossen

Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, voert u de volgende stappen uit:

- De meeste problemen met de installatie van DKIM hebben betrekking op onjuiste DNS-records. Controleer of de DKIM CNAME-record (**geen** TXT-record) correct is opgemaakt. Zie het volgende [onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)voor meer informatie.

- Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistratie), wacht dan totdat de DNS-records zijn doorgegeven.

- Als u de DNS-records van DKIM niet kunt maken in het Beheercentrum, kunt u \<CustomDomain\> deze vervangen door uw aangepaste domein (bijvoorbeeld contoso.com) en deze opdracht uit te voeren in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
