---
title: Het oplossen van toegang tot berichten van OneDrive voor bedrijven-sites is geweigerd
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670611"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Het oplossen van toegang tot berichten van OneDrive voor bedrijven-sites is geweigerd

Dit probleem treedt vaak op wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met de UPN (User Principal Name) van de gebruiker. Het nieuwe account wordt gemaakt met behulp van een andere PUID-waarde (Passport unieke ID). Wanneer de gebruiker een siteverzameling of de OneDrive probeert te openen, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid van Active Directory. Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kan dit probleem zich voordoen.

1. Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Als u de oorspronkelijke gebruiker niet kunt terugzetten, verwijdert u de gebruikers uit de OneDrive-site met deze stappen, [verwijdert u een gebruiker uit de lijst gebruikersinfo](). 
3. Wanneer dit is gebeurd, kunt u controleren of de gebruiker beheerdersrechten heeft voor de OneDrive-site door de stappen te volgen voor het [toevoegen van beheerders voor onedrive van een gebruiker](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Zie het artikel [over machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)voor meer informatie over machtigingsniveaus.
