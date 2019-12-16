---
title: Toegang tot pensioendiensten
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050484"
---
# <a name="access-services-retirement"></a>Toegang tot pensioendiensten

Zoals we oorspronkelijk aankondigden in MC97576, in maart 2017, en bleven communiceren over het afgelopen jaar, worden de toegangsdiensten buiten gebruik gesteld van Office 365. De volgende fase in dit proces is het verwijderen van Access Web-databases die gebruikmaken van SharePoint-lijsten als onderliggende gegevensopslag.

**Hoe beïnvloedt dit mij?**

Vanaf juni 2019 zullen we stoppen met het maken van nieuwe Access-databases in SharePoint Online en de service en eventuele resterende apps afsluiten door 2020 april.

**Wat moet ik doen om voor te bereiden op deze wijziging?**

We raden u aan een overgangsplan voor de Access-webdatabases van uw organisatie te maken. Beheerders kunnen de [SharePoint Access app-scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris op te vragen van de Access-apps die sites gebruiken.

Er zijn verschillende manieren om gegevens van Access-webdatabases te migreren:

- Importeren in een lokale Access-database (. ACCDB) of naar een Excel-bestand.
- We raden u ook aan Microsoft PowerApps te verkennen als alternatief platform voor het maken van niet-code zakelijke oplossingen voor web-en mobiele apparaten.