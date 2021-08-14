---
title: Een verwijderde Microsoft 365 herstellen
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959021"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Een verwijderde Microsoft 365 herstellen

U kunt een verwijderde groep Microsoft 365 of Microsoft Teams binnen 30 dagen na de verwijdering herstellen.

1. Ga naar de [Microsoft 365-beheercentrum](https://aka.ms/RestoreDeletedGroup) om u aan te melden bij een lijst met de verwijderde groepen en teams.

    **Opmerking:** Meld u aan met het account dat is toegewezen aan de tenantbeheerder of de beheerdersrol voor groepen.

1. Selecteer de verwijderde Microsoft 365/Teams die u wilt herstellen en klik op **groep herstellen.**

    Als de groep niet kan worden hersteld vanwege een conflicterend SMTP-adres, gebruikt u de volgende opdracht om het object te zoeken dat conflict veroorzaakt en het SMTP-adres te verwijderen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Opmerking:** In sommige gevallen kan het 24 uur duren voordat de groep en alle gegevens zijn hersteld.

    Zie Een verwijderde groep herstellen voor meer [Microsoft 365 informatie of](https://go.microsoft.com/fwlink/?linkid=867802)voor meer informatie over het herstellen van groepen met PowerShell.