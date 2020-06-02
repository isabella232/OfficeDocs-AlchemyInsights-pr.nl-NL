---
title: Problemen met geweigerde berichten met toegang oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505374"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen met geweigerde berichten oplossen in Sharepoint/OneDrive-beheercentrum

Als u een bericht met geweigerde toegang ontvangt wanneer u probeert naar een Sharepoint/OneDrive-beheercentrum te bladeren, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat aan de gebruiker [een beheerdersrol](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) wordt toegewezen die toegang heeft tot de beheercentra.

Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde naam van de gebruiker (UPN). Het nieuwe account wordt gemaakt met behulp van een andere PUID (Passport Unique ID) waarde. Wanneer de gebruiker toegang probeert te krijgen tot een siteverzameling of zijn/haar OneDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een Organisatie-eenheid (Active Directory organizational unit). Als gebruikers zich al hebben aangemeld bij SharePoint en vervolgens naar een andere organisatie worden verplaatst en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ondervinden.

Als u dit probleem wilt oplossen, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.  [Controleer het dashboard servicestatus](https://portal.office.com/adminportal/home#/servicehealth).


