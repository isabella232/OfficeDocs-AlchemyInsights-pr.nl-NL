---
title: Problemen met geweigerde toegangs berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051420"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen met toegang geweigerd berichten in SharePoint/OneDrive Admin Center oplossen

Als u een bericht toegang geweigerd ontvangt wanneer u probeert te bladeren naar een Admin Center van SharePoint/OneDrive, zorg ervoor dat u [een licentie toewijzen aan de gebruiker](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Als de gebruiker een licentie heeft, moet u ook ervoor zorgen dat ze [een beheerdersrol](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) die toegang hebben tot de admin Centers worden toegewezen.

Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw gemaakt met de dezelfde UPN (User Principal Name). De nieuwe account wordt gemaakt met behulp van een andere waarde van de PUID (paspoort unieke ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuiste PUID. Een tweede scenario heeft betrekking op adreslijstsynchronisatie met een Active Directory-organisatie-eenheid (OE). Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kunnen dit probleem optreden.

U lost dit probleem, moet u de oorspronkelijke UPN herstellen met de stappen in het artikel [herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Opmerking: als een OneDrive-of SharePoint-Beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.  [Controleer de servicestatus dashboard](https://portal.office.com/adminportal/home#/servicehealth).


