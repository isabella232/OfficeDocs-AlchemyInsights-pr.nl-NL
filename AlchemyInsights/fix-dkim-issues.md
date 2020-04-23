---
title: Problemen met de installatie van DKIM oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717557"
---
# <a name="fix-dkim-setup-issues"></a>Problemen met de installatie van DKIM oplossen

Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, gebruikt u de volgende stappen:

- De meeste problemen met de installatie van DKIM zijn gerelateerd aan onjuiste DNS-records. Controleer of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt. Zie dit [onderwerp](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)voor meer informatie.

- Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistrar), wacht u tot de DNS-records worden gepropageerd.

- Als u de DKIM DNS-records niet maken \<in\> het beheercentrum, u CustomDomain vervangen door uw aangepaste `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`domein (bijvoorbeeld contoso.com) en deze opdracht uitvoeren in Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).
