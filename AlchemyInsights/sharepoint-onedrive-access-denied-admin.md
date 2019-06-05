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
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716642"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problemen oplossen met berichten in Sharepoint OneDrive/Admin Center toegang geweigerd

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Als u toegang geweigerd tijdens een poging om te bladeren naar een Sharepoint OneDrive/Admin Center ontvangt, moet u controleren dat u <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">een licentie voor de gebruiker toewijzen </a>. Als de gebruiker een licentie heeft, moet u ervoor dat ze <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">een rol toegewezen aan</a> die toegang heeft tot de admin-centers.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Dit probleem kan ook optreden wanneer een gebruiker is verwijderd en opnieuw met de dezelfde UPN (User Principal Name gemaakt). De nieuwe account is gemaakt met behulp van een andere waarde voor de PUID (unieke Passport-ID). Wanneer de gebruiker probeert toegang te krijgen tot een siteverzameling of hun OneDrive, heeft de gebruiker een onjuist PUID. Een tweede scenario heeft betrekking op directory synchronisatie met een organisatie-eenheid (OU) van Active Directory. Als gebruikers hebben al aangemeld bij SharePoint, worden verplaatst naar een andere organisatie-eenheid en resynced met SharePoint, kunnen zij dit probleem optreden.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Dit probleem op te lossen moet u weer de oorspronkelijke UPN met de stappen in het artikel, het <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">herstellen van een gebruiker in Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Opmerking:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">als een OneDrive of SharePoint Admin center niet beschikbaar voor meerdere gebruikers die eerder toegang had is, is er mogelijk een probleem tijdelijke service.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Controleert de gezondheid servicedashboard</span></a>.</span></em></span></span></p>


