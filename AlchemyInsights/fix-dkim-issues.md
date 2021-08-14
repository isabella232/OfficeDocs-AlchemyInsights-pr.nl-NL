---
title: Problemen met het instellen van DKIM oplossen
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945926"
---
# <a name="fix-dkim-setup-issues"></a>Problemen met het instellen van DKIM oplossen

Als u problemen hebt met het inschakelen van DKIM voor uw aangepaste domein, gebruikt u de volgende stappen:

- De meeste DKIM-installatieproblemen zijn gerelateerd aan onjuiste DNS-records. Controleer of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt. Zie dit onderwerp voor [meer informatie.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistrar), wacht u totdat de DNS-records worden doorgegeven.

- Als u de DKIM DNS-records niet kunt maken in het beheercentrum, kunt u het aangepaste domein (bijvoorbeeld contoso.com) vervangen en deze opdracht uitvoeren \<CustomDomain\> in [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
