---
title: Access services pensioen
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973910"
---
# <a name="access-services-retirement"></a>Access services pensioen

Zoals oorspronkelijk aangekondigd in MC97576, in maart 2017, en we communiceren in het afgelopen jaar wederom wordt toegang tot Services van Office 365 teruggetrokken. De volgende fase in dit proces is het verwijderen van Databases van Access Web die SharePoint-lijsten als hun onderliggende gegevensopslag gebruiken.

## <a name="how-does-this-affect-me"></a>Wat betekent dit voor mij?

Begin juni 2019, we stoppen met het maken van een nieuwe Access-databases in SharePoint Online en de service en eventuele resterende apps afsluiten in April 2020.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Wat moet ik doen als voorbereiding op deze wijziging?

We raden u aan een overgang maken voor Access web-databases van de organisatie. Beheerders kunt de [toegang tot SharePoint app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) ophalen een inventarisatie van de toegang tot toepassingen die door sites wordt gebruikt. 

Er zijn verschillende manieren om gegevens van Access web databases te migreren:

- Importeren van een lokale Access-database (. ACCDB-bestand) of een Excel-bestand.
- Ook wordt aangeraden Microsoft PowerApps verkennen als een alternatief platform zonder code zakelijke oplossingen voor web en mobiele apparaten maken.