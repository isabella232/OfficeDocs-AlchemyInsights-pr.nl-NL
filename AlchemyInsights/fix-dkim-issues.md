---
title: DKIM-installatieproblemen oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764977"
---
# <a name="fix-dkim-setup-issues"></a>DKIM-installatieproblemen oplossen

Als u problemen hebt met het DKIM inschakelen voor uw aangepaste domein, gebruikt u de volgende stappen uit:

- De meeste problemen bij de installatie DKIM zijn gerelateerd aan een onjuiste DNS-records. Controleer of dat de DKIM CNAME-record (**niet** een TXT-record) juist is opgemaakt. Raadpleeg dit [onderwerp](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)voor meer informatie.

- Na het maken of bijwerken uw DKIM DNS-records op de DNS-hostingservice voor uw domein (meestal uw domeinregistratieservice), wachten op de DNS-records doorgeven.

- Als u geen DKIM DNS records in het beheercentrum maken, vervangt u \<CustomDomain\> met uw aangepaste domein (bijvoorbeeld contoso.com) en voer deze opdracht uit in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
