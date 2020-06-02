---
title: Problemen met geweigerde berichten openen naar OneDrive voor Bedrijven-sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511179"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problemen met geweigerde berichten openen naar OneDrive voor Bedrijven-sites

Dit probleem treedt het vaakst op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde naam van de gebruiker (UPN). Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde. Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn/haar OneDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een Organisatie-eenheid (Active Directory organizational unit). Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatie worden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.

1. Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker met deze stappen verwijderen van de OneDrive-site, [een gebruiker uit de lijst met gebruikersgegevens verwijderen.]() 
3. Nadat dit is gedaan, u controleren of de gebruiker beheerdersrechten heeft voor de OneDrive-site door de stappen te volgen naar [Beheerders toevoegen voor de OneDrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Zie het artikel [Machtigingsniveaus in SharePoint voor](https://docs.microsoft.com/sharepoint/understanding-permission-levels)meer informatie over machtigingsniveaus.
