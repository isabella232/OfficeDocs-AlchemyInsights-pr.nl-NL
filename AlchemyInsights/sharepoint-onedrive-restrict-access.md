---
title: Toegang beperken in SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700450"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Toegang beperken in SharePoint of OneDrive

Er zijn verschillende manieren om toegang tot SharePoint Online/OneDrive-services te beperken. Hieronder ziet u een overzicht van de verschillende restrictie methoden. 

**Machtigingsbeperking**

In SharePoint Online en OneDrive voor bedrijven beperkt u de toegang tot items, zoals sites, bestanden en mappen, alleen toegang tot de groepen en personen die toegang moeten hebben.

- [Machtigingen voor een SharePoint-lijst of-bibliotheek aanpassen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-site machtigingen aanpassen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [De machtigingen voor een submap wijzigen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Toegang beheren vanaf niet-beheerde apparaten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint-of globale beheerder kunt u de toegang tot SharePoint-en OneDrive-inhoud van niet-beheerde apparaten blokkeren of beperken (niet-hybride aantekening of compatibel met intune).

**Beperking van netwerklocatie**

Als IT-beheerder kunt u de toegang tot SharePoint-en OneDrive-bronnen beheren op basis van gedefinieerde netwerklocaties die u vertrouwt. Dit wordt ook wel het beleid op basis van locatie genoemd. Zie [toegang tot SharePoint Online en OneDrive-gegevens beheren op basis van netwerklocatie](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) voor meer informatie.

**Beperking site vergrendeling** 

In SharePoint Online kunt u de mogelijkheid van een siteverzameling vergrendelen, zodat niemand toegang heeft. Dit wordt ingesteld via PowerShell en de [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) met behulp van de eigenschap [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Voorkomen dat gebruikers sites of subsites maken**

Als SharePoint-beheerder of globale beheerder kunt u toestaan dat uw gebruikers hun eigen SharePoint-sites maken en beheren, bepalen welke soorten sites ze kunnen maken en de locatie van de sites opgeven. Zie [sites maken in SharePoint Online beheren](https://docs.microsoft.com/sharepoint/manage-site-creation) voor meer informatie.

