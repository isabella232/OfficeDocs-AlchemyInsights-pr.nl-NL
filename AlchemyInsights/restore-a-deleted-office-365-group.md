---
title: Een verwijderde Microsoft 365-groep herstellen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597438"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Een verwijderde Microsoft 365-groep herstellen

U kunt een verwijderde Microsoft 365-groep of Microsoft Teams binnen 30 dagen na de verwijdering herstellen.

1. Ga naar het [Microsoft 365-beheercentrum om](https://aka.ms/RestoreDeletedGroup) u aan te melden en de verwijderde groepen en teams op te nemen.

    **Opmerking:** Meld u aan met het account dat is toegewezen aan de tenantbeheerder of de beheerdersrol voor groepen.

1. Selecteer de verwijderde Microsoft 365-groep/Teams die u wilt herstellen en klik op **groep herstellen.**

    Als de groep niet kan worden hersteld vanwege een conflicterend SMTP-adres, gebruikt u de volgende opdracht om het object te zoeken dat conflict veroorzaakt en het SMTP-adres te verwijderen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Opmerking:** In sommige gevallen kan het 24 uur duren voordat de groep en alle gegevens zijn hersteld.

    Zie Een [verwijderde Microsoft 365-groep](https://go.microsoft.com/fwlink/?linkid=867802)herstellen voor meer informatie of voor meer informatie over het herstellen van groepen met PowerShell.