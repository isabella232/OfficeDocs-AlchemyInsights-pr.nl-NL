---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758393"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen met toegang geweigerde berichten oplossen in Sharepoint/OneDrive-beheercentrum

Als u een bericht met toegang geweigerd ontvangt wanneer u probeert te bladeren naar een Sharepoint/OneDrive-beheercentrum, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One) Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat deze [een beheerdersrol krijgt](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) toegewezen die toegang heeft tot de beheerderscentra.

Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde gebruikersnaam (UPN). Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde. Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn OfaDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OU). Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatieworden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.

Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel, [Een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijke serviceprobleem.  [Controleer het dashboard voor servicestatus](https://portal.office.com/adminportal/home#/servicehealth).


