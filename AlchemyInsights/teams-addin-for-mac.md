---
title: Teams invoeging voor Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940670"
---
# <a name="teams-add-in-for-mac"></a>Teams invoeging voor Mac

Als u een probleem wilt oplossen Teams gebruikers van een Mac-besturingssysteem, gaat u als volgt te werk:

**Stap 1:** Als u hybride Exchange on-premises (2016 CU3 of hoger vereist) hebt, gebruikt u het hulpprogramma Test-HMA.ps1 om te controleren of hybride moderne verificatie correct is geconfigureerd. Zie Valideren van hybride moderne verificatie voor Outlook [voor iOS en Android voor meer informatie.](https://aka.ms/TestHMAEAS)  

**Opmerking** Gebruik de UPN-adresnotatie [(bijvoorbeeld](mailto:username@contoso.com)username@contoso.com ), niet domein\gebruikersnaam. Doe dit zelfs voor gebruikers met Exchange Online postvakken.

**Stap 2:** Laat de gebruiker naar **Hulpmiddelenaccounts**  >  **gaan**... in Outlook voor Mac en het account zoeken en selecteren. Bevestig dat de gebruikersnaam die wordt vermeld, in UPN-indeling staat [(bijvoorbeeld username@contoso.com).](mailto:username@contoso.com)

**Stap 3:** Controleer of de gebruiker een gelicentieerde Microsoft Teams is. De gebruiker moet het abonnement Office 365 voor Mac, productversie 16.24 of hoger gebruiken.