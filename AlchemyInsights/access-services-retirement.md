---
title: Toegang tot diensten pensionering
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
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687253"
---
# <a name="access-services-retirement"></a>Toegang tot diensten pensionering

Zoals we oorspronkelijk aangekondigd in MC97576, in maart 2017, en bleef communiceren in het afgelopen jaar Access Services worden teruggetrokken. De volgende fase in dit proces is het verwijderen van Access Web Databases die SharePoint-lijsten gebruiken als onderliggende gegevensopslag.

**Wat voor invloed heeft dit op mij?**

Vanaf juni 2019 stoppen we met het maken van nieuwe Access-databases in SharePoint Online en sluiten we de service en de resterende apps af in april 2020.

**Wat moet ik doen om me voor te bereiden op deze verandering?**

We raden u aan een overgangsplan te maken voor de Access-webdatabases van uw organisatie. Beheerders kunnen de [SharePoint Access-app-scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris te krijgen van de Access-apps die sites gebruiken.

Er zijn verschillende manieren om Access-webdatabasesgegevens te migreren:

- Importeren in een lokale Access-database (. ACCDB) of naar een Excel-bestand.
- We raden u ook aan Microsoft PowerApps te verkennen als alternatief platform om bedrijfsno-codeoplossingen voor web- en mobiele apparaten te maken.