---
title: Problemen met DKIM-instellingen oplossen
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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506769"
---
# <a name="fix-dkim-setup-issues"></a>Problemen met DKIM-instellingen oplossen

Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, voert u de volgende stappen uit:

- De meeste DKIM-installatieproblemen zijn gerelateerd aan onjuiste DNS-records. Controleer of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt. Zie dit onderwerp [voor](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)meer informatie.

- Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistrar), wacht u tot de DNS-records zijn doorgegeven.

- Als u de DNS-records van DKIM niet maken in het beheercentrum, u \<CustomDomain\> uw aangepaste domein (bijvoorbeeld contoso.com) vervangen en deze opdracht uitvoeren in Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
