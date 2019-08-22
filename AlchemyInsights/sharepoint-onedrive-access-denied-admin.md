---
title: Problemen oplossen met berichten die de toegang geweigerd
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503522"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen oplossen met berichten in Sharepoint OneDrive/Admin Center toegang geweigerd

Als u toegang geweigerd tijdens een poging om te bladeren naar een Sharepoint OneDrive/Admin Center ontvangt, moet u controleren dat u [een licentie voor de gebruiker toewijzen](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Als de gebruiker een licentie heeft, moet u ervoor dat ze [een rol toegewezen aan](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) die toegang heeft tot de admin-centers.

Dit probleem kan ook optreden wanneer een gebruiker is verwijderd en opnieuw met de dezelfde UPN (User Principal Name gemaakt). De nieuwe account is gemaakt met behulp van een andere waarde voor de PUID (unieke Passport-ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuist PUID. Een tweede scenario heeft betrekking op directory synchronisatie met een organisatie-eenheid (OU) van Active Directory. Als gebruikers hebben al aangemeld bij SharePoint, worden verplaatst naar een andere organisatie-eenheid en resynced met SharePoint, kunnen zij dit probleem optreden.

Dit probleem op te lossen moet u weer de oorspronkelijke UPN met de stappen in het artikel, het [herstellen van een gebruiker in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Opmerking: Als een OneDrive of SharePoint Admin center niet beschikbaar voor meerdere gebruikers die eerder toegang had is, kan er een tijdelijke service-probleem.  [Controleer de gezondheid servicedashboard](https://portal.office.com/adminportal/home#/servicehealth).


