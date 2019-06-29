---
title: Access services pensioen
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359336"
---
# <a name="access-services-retirement"></a>Access services pensioen

Zoals oorspronkelijk aangekondigd in MC97576, in maart 2017, en we communiceren in het afgelopen jaar wederom wordt toegang tot Services van Office 365 teruggetrokken. De volgende fase in dit proces is het verwijderen van Databases van Access Web die SharePoint-lijsten als hun onderliggende gegevensopslag gebruiken.

**Wat betekent dit voor mij?**

Begin juni 2019, we stoppen met het maken van een nieuwe Access-databases in SharePoint Online en de service en eventuele resterende apps afsluiten in April 2020.

**Wat moet ik doen als voorbereiding op deze wijziging?**

We raden u aan een overgang maken voor Access web-databases van de organisatie. Beheerders kunt de [toegang tot SharePoint app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) ophalen een inventarisatie van de toegang tot toepassingen die door sites wordt gebruikt.

Er zijn verschillende manieren om gegevens van Access web databases te migreren:

- Importeren van een lokale Access-database (. ACCDB-bestand) of een Excel-bestand.
- Ook wordt aangeraden Microsoft PowerApps verkennen als een alternatief platform zonder code zakelijke oplossingen voor web en mobiele apparaten maken.