---
title: Problemen met toegang tot berichten geweigerd voor OneDrive voor Business-sites
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354792"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problemen met toegang tot berichten geweigerd voor OneDrive voor Business-sites

Dit probleem treedt meestal op wanneer een gebruiker is verwijderd en opnieuw met de dezelfde UPN (User Principal Name gemaakt). De nieuwe account is gemaakt met behulp van een andere waarde voor de PUID (unieke Passport-ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuist PUID. Een tweede scenario heeft betrekking op directory synchronisatie met een organisatie-eenheid (OU) van Active Directory. Als gebruikers hebben al aangemeld bij SharePoint, worden verplaatst naar een andere organisatie-eenheid en resynced met SharePoint, kunnen zij dit probleem optreden.

Om dit probleem te verhelpen moet u weer de oorspronkelijke UPN met de stappen in het artikel, het[herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nadat dit is gebeurd, kunt u controleren of dat de gebruiker heeft admin rechten op de OneDrive website met de volgende stappen om [admin toevoegen voor OneDrive van de gebruiker de](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Zie voor meer informatie over machtigingsniveaus, het artikel, [Wat zijn machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
