---
title: Toegang beperken in SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053760"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Toegang beperken in SharePoint of OneDrive

Er zijn veel manieren om de toegang tot SharePoint Online/OneDrive-services te beperken. Deze verschillende methoden voor toegangsbeperking worden hieronder beschreven. 

**Beperking van machtigingen**

In SharePoint Online en OneDrive voor bedrijven beperken we de toegang tot items zoals sites, bestanden en mappen door alleen toegang te verlenen aan die groepen/personen die toegang moeten hebben.

- [Machtigingen voor een SharePoint-lijst of-bibliotheek aanpassen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-site machtigingen aanpassen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [De machtigingen voor een submap wijzigen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Toegang beheren vanaf niet-beheerde apparaten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als een SharePoint of globale beheerder in Office 365, u blokkeren of beperken van toegang tot SharePoint en OneDrive-inhoud van niet-beheerde apparaten (die niet hybride AD toegevoegd of compatibel zijn in intune).

**Beperking van netwerklocatie**

Als IT-beheerder u de toegang tot SharePoint-en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt. Dit wordt ook wel op locatie gebaseerd beleid genoemd. Voor meer informatie raadpleegt u [toegang tot SharePoint Online en OneDrive-gegevens beheren op basis van netwerklocatie](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Beperking van site vergrendeling** 

In SharePoint Online hebt u de mogelijkheid om een siteverzameling te vergrendelen, zodat niemand toegang heeft. Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate eigenschap.

**Gebruikers beperken om sites of subsites te maken**

Als SharePoint-beheerder of Office 365 globale beheerder u uw gebruikers hun eigen SharePoint-sites laten maken en beheren, bepalen wat voor soort sites ze kunnen maken en de locatie van de sites opgeven. Zie voor meer informatie, [site maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation)

