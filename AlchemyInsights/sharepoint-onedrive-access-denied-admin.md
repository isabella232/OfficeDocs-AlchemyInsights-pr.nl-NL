---
title: Problemen met toegang geweigerde berichten oplossen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707949"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen met toegang geweigerde berichten in sharepoint/OneDrive-beheercentrum oplossen

Als u een bericht ontvangt dat de toegang is geweigerd wanneer u naar een Sharepoint/OneDrive-beheercentrum bladert, moet u ervoor zorgen dat u een licentie [toewijst aan de gebruiker.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Als de gebruiker een licentie heeft, moet [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) u er ook voor zorgen dat aan de gebruiker een beheerdersrol is toegewezen die toegang heeft tot de beheercentra.

Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met dezelfde USER PRINCIPAL Name (UPN). Het nieuwe account wordt gemaakt met behulp van een andere waarde voor de PUID (Passport Unique ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of oneDrive, beschikt de gebruiker over een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid (OU) van Active Directory. Als gebruikers zich al hebben aangemeld bij SharePoint, en vervolgens worden verplaatst naar een andere OU en opnieuw worden gesynchroniseerd met SharePoint, kunnen ze dit probleem ervaren.

U kunt dit probleem oplossen door de oorspronkelijke UPN te herstellen volgens de stappen in het artikel, Een gebruiker [herstellen in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Opmerking: Als een OneDrive- of SharePoint-beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.  [Bekijk het dashboard voor de service status.](https://portal.office.com/adminportal/home#/servicehealth)


