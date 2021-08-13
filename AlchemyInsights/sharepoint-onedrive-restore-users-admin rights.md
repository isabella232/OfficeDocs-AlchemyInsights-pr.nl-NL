---
title: Problemen met Access-geweigerde berichten oplossen OneDrive voor Bedrijven sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957788"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problemen met Access-geweigerde berichten oplossen OneDrive voor Bedrijven sites

Dit probleem treedt het meest op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde gebruikersnaam (UPN). Het nieuwe account wordt gemaakt met behulp van een andere PUID-waarde (Unieke paspoort-id). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of de OneDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario bestaat uit adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OU). Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere OU en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ervaren.

1. Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel: Een gebruiker [terugzetten in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Als u de oorspronkelijke gebruiker niet kunt herstellen, verwijdert u de oude gebruiker van de OneDrive site met deze stappen, Verwijdert u een gebruiker uit de lijst [met gebruikersgegevens.]() 
3. Nadat dit is gedaan, kunt u controleren of de gebruiker beheerdersrechten heeft [](https://docs.microsoft.com/sharepoint/manage-user-profiles) voor de OneDrive-site door de stappen te volgen voor Beheerders toevoegen voor de OneDrive

Zie het artikel Machtigingsniveaus in SharePoint voor [meer informatie over machtigingsniveaus.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
