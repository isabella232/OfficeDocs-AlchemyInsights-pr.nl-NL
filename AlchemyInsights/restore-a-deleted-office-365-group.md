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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645126"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Een verwijderde Microsoft 365-groep herstellen

U kunt een verwijderde Microsoft 365-groep of Microsoft Teams binnen 30 dagen na de verwijdering herstellen.

1. Ga naar het [Microsoft 365-beheercentrum](https://aka.ms/RestoreDeletedGroup) om u aan te melden bij een lijst met de verwijderde groepen en teams.

    **Opmerking:** Meld u aan met het account dat is toegewezen aan de tenantbeheerder of de beheerdersrol voor groepen.

1. Selecteer de verwijderde Microsoft 365-groep/Teams die u wilt herstellen en klik op **groep herstellen.**

    Als de groep niet kan worden hersteld vanwege een conflicterend SMTP-adres, gebruikt u de volgende opdracht om het object te zoeken dat conflict veroorzaakt en het SMTP-adres te verwijderen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Opmerking:** In sommige gevallen kan het 24 uur duren voordat de groep en alle gegevens zijn hersteld.

    Zie Een [verwijderde Microsoft 365-groep](https://go.microsoft.com/fwlink/?linkid=867802)herstellen voor meer informatie of voor meer informatie over het herstellen van groepen met PowerShell.