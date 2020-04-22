---
title: Probleemoplossing Toegang geweigerde berichten naar OneDrive voor Bedrijven-sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692796"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Probleemoplossing Toegang geweigerde berichten naar OneDrive voor Bedrijven-sites

Dit probleem treedt het vaakst op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde gebruikersnaam (UPN). Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde. Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn OfaDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OU). Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatieworden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.

1. Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker met deze stappen van de OneDrive-site verwijderen, [een gebruiker verwijderen uit de lijst met gebruikersgegevens](). 
3. Nadat dit is gebeurd, u controleren of de gebruiker beheerdersrechten heeft op de OneDrive-site door de stappen te volgen om beheerders toe te [voegen voor de OneDrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Zie het artikel [Machtigingsniveaus in SharePoint voor](https://docs.microsoft.com/sharepoint/understanding-permission-levels)meer informatie over machtigingsniveaus.
