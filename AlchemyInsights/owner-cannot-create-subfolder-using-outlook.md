---
title: Eigenaar kan geen submap maken door Outlook te gebruiken
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836130"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Eigenaar kan geen submap maken door Outlook te gebruiken

**Er is een voortdurend probleem met openbare eigenaren van mappen die submappen maken door Outlook te gebruiken. Het probleem wordt snel opgelost.**

Ondertussen kunt u een de volgende tijdelijke oplossingen gebruiken:

1. Gebruik Outlook voor Mac om submappen te maken, omdat het probleem zich alleen voordoet bij Outlook voor desktop windows (alle versies)
2. Laat de beheerder de submap maken door EXO Shell of EAC te gebruiken
3. Wijzig DefaultPublicFolderMailbox/EffectivePublicFolderMailbox van de gebruiker naar een ander postvak dan de Inhoud Mailbox voor de map die voor problemen zorgt  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Wacht een uur en start dan outlook cliënt opnieuw op