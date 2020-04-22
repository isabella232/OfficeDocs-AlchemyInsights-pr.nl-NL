---
title: Toegang in SharePoint of OneDrive beperken
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692760"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Toegang in SharePoint of OneDrive beperken

Er zijn veel manieren om de toegang tot SharePoint Online/OneDrive-services te beperken. Deze verschillende toegangsbeperkingsmethoden worden hieronder beschreven. 

**Machtigingsbeperking**

In SharePoint Online en OneDrive voor Bedrijven beperken we de toegang tot items zoals sites, bestanden en mappen door alleen toegang te verlenen aan groepen/personen die toegang moeten hebben.

- [Machtigingen aanpassen voor een SharePoint-lijst of -bibliotheek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-site machtigingen aanpassen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [De machtigingen voor een submap wijzigen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Toegang beheren vanaf niet-beheerde apparaten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint- of globale beheerder u de toegang tot SharePoint- en OneDrive-inhoud vanaf niet-beheerde apparaten blokkeren of beperken (die niet hybride AD hebben samengevoegd of in Intune zijn compatibel).

**Beperking van de netwerklocatie**

Als IT-beheerder u de toegang tot SharePoint- en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt. Dit wordt ook wel locatiegebaseerd beleid genoemd. Zie Toegang tot [SharePoint Online- en OneDrive-gegevens](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) beheren op basis van netwerklocatie voor meer informatie.

**Beperking sitevergrendeling** 

Binnen SharePoint Online hebt u de mogelijkheid om een siteverzameling te vergrendelen, zodat niemand toegang heeft. Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de eigenschap [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Gebruikers beperken om sites of subsites te maken**

Als SharePoint-beheerder of globale beheerder u uw gebruikers hun eigen SharePoint-sites laten maken en beheren, bepalen wat voor soort sites ze kunnen maken en de locatie van de sites opgeven. Zie [Sitemaken van de site beheren in SharePoint Online beheren voor](https://docs.microsoft.com/sharepoint/manage-site-creation) meer informatie

