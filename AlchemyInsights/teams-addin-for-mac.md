---
title: Invoegtoepassing teams voor Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629491"
---
# <a name="teams-add-in-for-mac"></a>Invoegtoepassing teams voor Mac

Voer de volgende stappen uit als u een ontbrekende invoegtoepassing voor teams voor een Mac-besturingssysteem wilt problemen:

**Stap 1:** Als u een hybride Exchange on-premises (2016 CU3 of hoger) hebt, gebruikt u het hulpprogramma Test-HMA.ps1 om te controleren of de hybride moderne verificatie correct is geconfigureerd. Zie [hybride instellingen voor moderne verificatie valideren voor Outlook voor IOS en Android](https://aka.ms/AA980zq)voor meer informatie.  

**Opmerking** Gebruik de notatie voor de UPN-adres (bijvoorbeeld [username@contoso.com](mailto:username@contoso.com)), niet DOMEIN\gebruikersnaam. Doe dit ook voor gebruikers met postvakken van Exchange Online.

**Stap 2:** Laat de gebruiker naar **extra**  >  **accounts**gaan... in Outlook voor Mac, zoekt en selecteert u het account. Controleer of de naam van de gebruikersnaam in de weergegeven UPN-indeling is (bijvoorbeeld [username@contoso.com](mailto:username@contoso.com)).

**Stap 3:** Controleer of de gebruiker een licentie heeft voor Microsoft teams. De gebruiker moet het Office 365 voor Mac-abonnement, productversie 16,24 of hoger, gebruiken.