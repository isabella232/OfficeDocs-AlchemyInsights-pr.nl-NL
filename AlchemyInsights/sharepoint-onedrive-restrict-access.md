---
title: Beperk de toegang in de SharePoint- of OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559872"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Beperk de toegang in de SharePoint- of OneDrive

Er zijn veel manieren om toegang te beperken tot SharePoint Online/OneDrive services. Deze verschillende methoden beperking worden hieronder nader belicht. 

**Beperking van de machtiging**

In SharePoint Online en OneDrive voor Business beperken we toegang tot objecten, zoals sites, bestanden en mappen door alleen toegang verlenen tot de groepen/personen die toegang moeten hebben.

- [Machtigingen voor een SharePoint-lijst of bibliotheek aanpassen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Machtigingen voor SharePoint-site aanpassen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [De machtigingen voor een submap](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Toegang beheren vanaf niet-beheerde apparaten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint of globale admin in Office 365, kunt u blokkeren of beperken van toegang tot SharePoint en OneDrive inhoud van niet-beheerde apparaten (die geen hybride AD gekoppelde of compatibele in Intune).

**Netwerk locatie beperking**

Als IT-beheer kunt u toegang tot bronnen van SharePoint en OneDrive op basis van gedefinieerde netwerklocaties die u vertrouwt. Dit is ook bekend als beleid op basis van locatie. Zie voor meer informatie, [toegang tot SharePoint Online en OneDrive gegevens op basis van locatie beheren](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Sitebeperking vergrendelen** 

U hebt de mogelijkheid een siteverzameling vergrendelen zodat niemand toegang heeft in SharePoint Online. Dit wordt ingesteld via PowerShell en [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met de eigenschap [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.

**Voorkomen dat gebruikers kunnen sites of subsites maken**

Als een beheerder van SharePoint of Office 365 globale beheerder kunt u uw gebruikers maken en beheren van hun eigen SharePoint-sites, bepalen wat voor soort sites kunnen maken, en geef de locatie van de sites. Zie voor meer informatie, [maken van de site beheren in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

