---
title: De uittreding van Access-services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938690"
---
# <a name="access-services-retirement"></a>De uittreding van Access-services

Zoals we oorspronkelijk hebben aangekondigd in MC97576, in maart 2017, en het afgelopen jaar is de Access Services niet meer gebruikt. De volgende fase in dit proces is het verwijderen van Access Web Databases die SharePoint gebruiken als onderliggende gegevensopslag.

**Wat voor invloed heeft dit op mij?**

Vanaf juni 2019 stoppen we met het maken van nieuwe Access-databases in SharePoint Online en sluiten we de service en eventuele resterende apps af in april 2020.

**Wat moet ik doen om deze wijziging voor te bereiden?**

We raden u aan een overgangsplan te maken voor de Access-webdatabases van uw organisatie. Beheerders kunnen de scanner SharePoint [Access-app gebruiken](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) om een inventaris op te maken van de Access-apps die sites gebruiken.

Er zijn verschillende manieren om access-webdatabasesgegevens te migreren:

- Importeren in een lokale Access-database (. ACCDB) of naar een Excel bestand.
- We raden u ook aan om Microsoft PowerApps te verkennen als een alternatief platform om bedrijfsoplossingen zonder code te maken voor web- en mobiele apparaten.