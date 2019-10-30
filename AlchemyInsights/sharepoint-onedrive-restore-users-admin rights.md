---
title: Problemen met toegang geweigerd berichten naar OneDrive voor bedrijven-sites
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766706"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problemen met toegang geweigerd berichten naar OneDrive voor bedrijven-sites

Dit probleem treedt meestal op wanneer een gebruiker wordt verwijderd en opnieuw gemaakt met de dezelfde UPN (User Principal Name). De nieuwe account wordt gemaakt met behulp van een andere waarde van de PUID (paspoort unieke ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario heeft betrekking op adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OE). Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kunnen dit probleem optreden.

1. Om dit probleem op te lossen moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [een gebruiker herstellen in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Als u de oorspronkelijke gebruiker niet herstellen, moet u de oude gebruiker uit de OneDrive-site verwijderen met behulp van deze stappen, [een gebruiker verwijderen uit de lijst met gebruikersgegevens](). 
3. Nadat dit is gebeurd, u controleren of de gebruiker beheerdersrechten heeft op de OneDrive-site door de stappen [voor het toevoegen van beheerders voor de onedrive van een gebruiker toe te voegen](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Zie voor meer informatie over machtigingsniveaus het artikel [machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
