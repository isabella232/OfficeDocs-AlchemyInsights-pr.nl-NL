---
title: Berichten voor geweigerde toegang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767656"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Berichten in de Access-Beheercentrum in SharePoint/OneDrive oplossen

Als u het bericht toegang geweigerd ontvangt wanneer u naar een SharePoint-Beheercentrum probeert te bladeren, moet u ervoor zorgen dat u [een licentie aan de gebruiker toewijst](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Als de gebruiker een licentie heeft, moet u er ook voor zorgen dat [aan de gebruiker een beheerdersrol is toegewezen](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) die toegang heeft tot de beheer centra.

Dit probleem kan ook optreden wanneer een gebruiker wordt verwijderd en opnieuw wordt gemaakt met de UPN (User Principal Name) van de gebruiker. Het nieuwe account wordt gemaakt met behulp van een andere PUID-waarde (Passport unieke ID). Wanneer de gebruiker een siteverzameling of de OneDrive probeert te openen, heeft de gebruiker een onjuiste PUID. Een tweede scenario omvat adreslijstsynchronisatie met een organisatie-eenheid van Active Directory. Als gebruikers al zijn aangemeld bij SharePoint en vervolgens worden verplaatst naar een andere organisatie-eenheid en opnieuw worden gesynchroniseerd met SharePoint, kan dit probleem zich voordoen.

U kunt dit probleem oplossen door de oorspronkelijke UPN te herstellen met de stappen in het artikel [een gebruiker herstellen in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Opmerking: als een OneDrive-of SharePoint-Beheercentrum niet beschikbaar is voor meerdere gebruikers die eerder toegang hadden, is er mogelijk een tijdelijk serviceprobleem.  [Controleer het dashboard servicestatus](https://portal.office.com/adminportal/home#/servicehealth).


